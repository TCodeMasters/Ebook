# eBooks - Sistema de Gestión de Libros Electrónicos

Este es un proyecto de gestión de libros electrónicos llamado **eBooks**. Sin embargo, actualmente el sistema está presentando algunos errores durante la instalación y ejecución, y necesitamos ayuda para resolverlos. 

## 🛠 Requisitos del Servidor

Antes de comenzar con la instalación, asegúrate de que tu servidor cumpla con los siguientes requisitos:

- **PHP 8.2**
- **MySQL 5.6+**
- **Intl PHP Extension**
- **OpenSSL PHP Extension**
- **PDO PHP Extension**
- **Mbstring PHP Extension**
- **Tokenizer PHP Extension**
- **XML PHP Extension**
- **Ctype PHP Extension**
- **JSON PHP Extension**

## 📥 Instalación de eBooks

### Paso 1: Extraer y Subir

Descomprime el paquete de archivo descargado. Cambia el nombre del directorio `eBook` al nombre que desees para tu directorio y sube el directorio al servidor web mediante FTP o el panel de control de tu servidor.

### Paso 2: Crear la Base de Datos

Crea una base de datos para eBook desde el panel de control de tu servidor. Si tu servidor tiene phpMyAdmin, también puedes crear la base de datos mediante phpMyAdmin.

### Paso 3: Ejecutar el Asistente de Instalación

Accede a la dirección de tu sitio web en el navegador y podrás ver el asistente de instalación.

**Nota:** Debes configurar el directorio raíz de tu servidor web para que apunte a la carpeta `public`.

---

## 🚨 Problemas conocidos

Actualmente, el sistema está presentando **errores al intentar iniciar**. Si el archivo `.env` está configurado en **desarrollo (development)**, se generan varios errores durante la ejecución del instalador.

### Errores comunes:

1. **El instalador no se abre**: A pesar de seguir todos los pasos de instalación, el instalador no se inicia correctamente.
2. **Errores de configuración**: Si se inicia con el entorno de desarrollo (`.env` en `development`), se generan errores adicionales relacionados con dependencias y configuración de entorno.

Estamos buscando ayuda de desarrolladores que puedan contribuir a identificar y corregir estos problemas para que el sistema funcione correctamente.

---

## 🙏 Cómo puedes ayudar

Si eres un desarrollador con experiencia en Laravel o sistemas PHP, ¡te necesitamos!

Algunas formas en las que puedes contribuir:

- Identificar y corregir los errores que se presentan al iniciar el sistema.
- Mejorar la documentación de instalación.
- Revisar las dependencias y asegurar que estén correctamente configuradas.

Si estás interesado en colaborar, por favor abre un **Pull Request** o contacta a través de los **Issues** para discutir los errores que has encontrado y cómo podríamos solucionarlos.

---

## 👨‍💻 Instalación local (Desarrolladores)

Si deseas probar el sistema localmente, sigue los siguientes pasos:

1. Clona este repositorio:
    ```bash
    git clone https://github.com/tu-usuario/ebook.git
    cd ebook
    ```

2. Instala las dependencias con Composer:
    ```bash
    composer install
    ```
   **Nota:** Las dependencias ya están incluidas en el archivo `composer.lock`, por lo que puedes instalar las versiones especificadas en ese archivo. Sin embargo, es libre albedrío si deseas actualizar las dependencias ejecutando `composer update`. **Ten en cuenta que actualizar las dependencias puede causar problemas si hay versiones incompatibles.**

3. Crea tu archivo `.env` basado en el `.env.example`:
    ```bash
    cp .env.example .env
    ```

4. Configura tu base de datos y otros parámetros en el archivo `.env`.

5. Ejecuta las migraciones de base de datos (si es necesario):
    ```bash
    php artisan migrate
    ```

6. Lanza el servidor de desarrollo:
    ```bash
    php artisan serve
    ```

Visita `http://127.0.0.1` para ver si el sistema funciona correctamente.


## 📬 Contacto

Si tienes alguna pregunta, sugerencia o descubriste un error, no dudes en abrir un **Issue** en este repositorio o ponerte en contacto conmigo directamente.

---

¡Gracias por tu ayuda y por contribuir al proyecto!
