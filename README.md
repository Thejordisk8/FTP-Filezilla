Instalación y configuración de un servidor FTP con FileZilla

 # Paso 1: Descargar FileZilla Server
1. Ve a la página oficial de **FileZilla**: [https://filezilla-project.org/download.php?type=server](https://filezilla-project.org/download.php?type=server).
2. Descarga la ultima versión de FileZilla Server.

# Paso 2: Instalación de FileZilla Server
1. Durante la instalación, selecciona las opciones predeterminadas, pero asegúrate de elegir **Iniciar el servicio de FileZilla Server automáticamente**.
2. Finaliza la instalación y ejecuta *FileZilla Server Interface*.

# Paso 3: Configuración del Servidor FTP
A. Crear un nuevo usuario
1. En la ventana principal de *FileZilla Server Interface*, haz clic en *Edit*+*Users*+*add*.
2. Crea tu nombre y contraseña.
4. En el panel izquierdo, selecciona el directorio donde deseas permitir que el usuario cargue o descargue archivos.*Shared folders*.

# B. Configurar el puerto FTP
1. En la ventana principal de *FileZilla Server Interface* y ve a *Edit > Settings*.
2. En *General settings*, configura el puerto de escucha (por defecto es el 21).

# C. Configurar la conexión remota
Si deseas acceder al servidor FTP desde otra red:
1. Asegúrate de que el puerto 21 esté abierto en tu firewall.
2. Redirige el puerto 21 en tu router hacia la IP local de tu servidor.


# Paso 4: Verificación de la instalación
1. Abre un cliente FTP como *FileZilla Client*.
2. Conéctate al servidor utilizando la *dirección IP* del servidor FTP, el *nombre_usuario* y *contraseña*.
3. Verifica que puedas cargar y descargar archivos sin problemas.

# Paso 5: Seguridad
1. Es recomendable usar *FTPS* (FTP sobre SSL/TLS) para cifrar las conexiones. *Settings > FTP over TLS settings*.
2. Configura un firewall para permitir solo conexiones desde direcciones IP específicas si es necesario.

# Conclusión
Con estos pasos, habrás instalado y configurado un servidor FTP con *FileZilla Server*. Asegúrate de mantener actualizado tu servidor,
utilizar prácticas de seguridad adecuadas para evitar accesos no autorizados.

# Recursos adicionales
- [FileZilla Documentation](https://wiki.filezilla-project.org/Documentation)
