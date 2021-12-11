# Triaje---netcore-5
Triaje y comparador de hashes creado en c# y .net 5

Versión inicial 1.0

[*] Uso
- Añade cuantos host necesites
- Añade uno a uno los archivos a comprobar que necesites
- Al añadir un archivo se añadira al host y se descargara por SFTP a la carpeta pertinente
- Al indicar [Check] el programa descargara otra version actual del archivo y comprobara si son iguales generando el SHA-512

[*] Actualizaciones pendientes
- Añadir y poder modificar un pull de archivos para poder añadirlos a cualquier host en un solo click
- Conexion de SSH por clave publica
- .
- .
- .

[*] Necesario saber
- El Host donde nos conectemos tiene que tener activo el servicio SSH
- El Usuario por el cual realizamos la conexión debe tener permisos de lectura en los archivos a comprobar

[*] Recomendaciones
- No usar usuarios root, administradores o sudoers
- El programa no guarda la contraseña en ningun archivo, tampoco en ninguna variable auxiliar y después de utilizarla directamente del objeto 
textArea se elimina la información de su texto para impedir en la medida de lo posible ataques de volcado de memoria.
- La carpeta que se utiliza para almacenar información y descargar los archivos es consultada por la variable de entorno [Application.UserAppDataPath]
[C:\Users\**USER**\AppData\Roaming\Triaje]

![Ejemplo](https://user-images.githubusercontent.com/6060930/145686677-69084787-e8db-48a6-af61-e2f008ad9070.PNG)
