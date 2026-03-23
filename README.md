
<p align="center">
    <a href="https://www.xgproyect.org/" target="_blank">
        <img align="center" src="https://xgproyect.org/wp-content/uploads/2019/10/xgp-new-logo-black.png" width="250px" title="XG Proyect" alt="xgp-logo">
    </a>
    <br>
    <strong>X</strong>treme <strong>G</strong>amez <strong>Proyect</strong>o
    <br>
    <strong>Clon de OGame de código abierto</strong>
</p>

Acerca de
=========

XG Proyect (XGP) es una aplicación web de código abierto, clon de OGame, diseñada para crear clones del popular juego OGame, ambientado en un vasto y cautivador universo espacial. Nuestro objetivo es ofrecer un paquete lo más similar posible al original, pero manteniendo su diseño original.

## Requisitos

- PHP 7.4 o superior
- MySQLi 5.7 o superior

## ¿Cómo obtener XG Proyect?

### Manualmente
Esta es la forma más simple y fácil si no eres una persona técnica. ¡Descargar e instalar XG Proyect será fácil! ;)

 1. Ve a [releases](https://github.com/XGProyect/XG-Proyect-v3.x.x/releases)
 2. Busca la última versión y luego haz clic en **assets** y finalmente busca el archivo `.zip`.
 3. Descomprime el archivo, verás 2 archivos y 1 carpeta.
 4. Busca el contenido de la carpeta `upload`, solo lo que está dentro de esta es necesario.
 5. Copia el contenido de la carpeta `upload` a la raíz de tu hosting. Hay archivos ocultos, asegúrate de que también se copien, especialmente el archivo `.htaccess`.
 6. Asegúrate de que PHP tenga permisos de escritura en el directorio `config` para el nuevo archivo de configuración.
 7. Si hiciste todo correctamente, cuando abras el sitio serás dirigido al directorio `install/`, si no, intenta con `public/install`.
 8. Usando docker, XAMPP o cualquier stack local que desees, coloca los archivos copiados en tu raíz.

### Composer
Composer es un gestor de paquetes y también una forma rápida de configurar tu proyecto.

1. Ejecuta
```

composer create-project xgproyect/xgproyect

```
2. Una vez que composer haya terminado de instalar todas las dependencias, puedes usar docker (ver abajo).

## ¿Cómo ejecutar XG Proyect?
### Docker
La forma más fácil de hacerlo es usando Docker.

```

docker-compose up

```

También puedes construir con diferentes versiones de PHP:
```

docker build -t xgproyect:7.4 --build-arg PHP_VERSION=7.4 .

```

O construir y ejecutar todo junto, especificando una **versión de PHP**:
```

docker-compose build --build-arg PHP_VERSION=8.2 && docker-compose up -d

```

Simplemente cambia la **versión de PHP** a cualquier otra **versión** que desees probar.

### Otras formas
- También son posibles otras opciones como XAMPP, o usarlo en tu propio hosting.

### Valores por defecto de conexión a la BD
```

host=db
user=root
password=root
db=xgp
prefix=xgp_

```

## MailHog
XGP utiliza MailHog y PHPMailer como herramientas para un mejor soporte de correo. MailHog te permite interceptar correos electrónicos **localmente** y recibirlos en un panel conveniente.

Lee nuestra <a href="https://github.com/XGProyect/XG-Proyect-v3.x.x/wiki/MailHog-usage-and-setup" target="_blank">guía de MailHog</a> para comenzar.

## ¿Quién está usando XG Proyect?
Estamos felices de ofrecer este software brindando a otros la posibilidad de tener un buen clon de OGame.
Por otro lado, es un placer ver a personas usando XG Proyect.
<a href="https://github.com/XGProyect/XG-Proyect-v3.x.x/issues" target="_blank">Crea un ticket</a> en GitHub para que pueda poner el logo de tu juego aquí.

<img align="center" src="https://xgproyect.org/wp-content/uploads/2019/10/xgp-new-logo-black.png" width="150px" title="XG Proyect" alt="xgp-logo">

## Apoyamos
Las siguientes son herramientas o frameworks que utilizamos para mejorar nuestra experiencia de codificación.

<p>
    <a href="https://codeigniter.com/" rel="nofollow">
        <img src="https://codeigniter.com/favicon.ico" alt="CodeIgniter" width="75px">
    </a>
    <a href="https://getcomposer.org/" rel="nofollow">
        <img src="https://getcomposer.org/img/logo-composer-transparent2.png" alt="Composer" width="75px">
    </a>
    <a href="https://www.phpdoc.org/" rel="nofollow">
        <img src="https://avatars0.githubusercontent.com/u/1239567?s=400&v=4" alt="PHPDocumentor" width="75px">
    </a>
    <a href="https://github.com/llaville/php-compat-info" rel="nofollow">
        <img src="https://avatars2.githubusercontent.com/u/364342?s=460&v=4" alt="PHP CompatInfo" width="75px">
    </a>
</p>

## Licencia
XG Proyect es un software de código abierto licenciado bajo la Licencia GPL-3.0.
