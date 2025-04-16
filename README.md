# Simple Bash

1. Abrir una terminal (`Ctrl + Alt + T`)
2. Crear una carpeta/directorio `tuia` en el `home` del usuario
3. Navegar/entrar al directorio `tuia`
4. Crear los archivos vacíos `hola` y `chau`
5. Editar con `nano` o `vim` el archivo `hola` y escribir en él `"Hola"`
6. Listar los archivos del directorio `tuia`
7. Listar TODOS los archivos del directorio `tuia`
> Ayuda: Ver la ayuda o el manual de `ls`
8. Crear un enlace simbólico a `hola` llamado `hello`
9. Crear un enlace duro a `hola` llamado `saludo`
> Ayuda: RTFM

10. Editar el archivo `hola`, de forma que se pueda ejecutar con el comando `bash` e imprima `Hola` en la terimal. 
11. Crear la siguiente estructura de archivos y directorios:
```
user@user:~/tuia $ tree
.
└── dir.a
    ├── dir.b
    │   ├── file.a
    │   └── file.b
    └── dir.c
        └── link.a -> ../dir.b/file.a

4 directories, 3 files 
```
12. a. Borrar el directorio `dir.a` y todo su contenido.
  b. Reescribir el ejercicio anterior intentando minimizar la cantidad de cambios de directorio (`cd`).

<div style="
    background-color: #fff3cd; 
    border-left: 5px solid #ffc107; 
    color: #856404; 
    padding: 15px; 
    margin: 10px 0; 
    border-radius: 4px; 
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    font-family: Arial, sans-serif;
">
    <div style="
        display: flex; 
        align-items: center; 
        margin-bottom: 10px;
    ">
        ⚠️ <strong style="
            font-size: 18px; 
            color: #856404;
            margin-left: 10px;
        ">Warning!</strong>
    </div>
    <p style="
        margin: 0; 
        line-height: 1.6;
    ">Los siguientes ejercicios exploran carpetas del sistema, resolverlos con conciencia.</p>
</div>

13. Listar los directorios del sistema, hay algunos archivos que llamen la atención? `Ver ejercicio 8`
> Ayuda: Recordá pasarle las opciones correcta a `ls` para que muestre más data.
14. Encontrar el kernel, dirigirnos hacia ese directorio e imprimir la ruta (`pwd`)
15. Explorar el contenido del directorio `/etc/`, qué tipos de archivos se encuentran allí?
16. Explorar el archivo `/etc/fstab`. Qué hace este archivo?
17. Buscar los comandos que corremos en la terminal. Por ejemplo, buscar dónde está `ls`.
> AYUDA: Son archivos **bin**arios (compilados) que están en algún directorio del sistema
18. Ejecutar el siguiente comando:
```
echo $PATH
```
Analizar su contenido e interpretar cómo se relaciona con el ejercicio anterior.
> AYUDA: Este ejercicio indaga un poco más en bash como lenguaje y sus configuraciones para usarlo en la terminal. Más adelante veremos como podemos usar y modificar esto.

## Usuarios, Grupos y Permisos

19. Crear un usuario `test_user`, verificar que el `home` del nuevo usuario se haya creado. (Si no se creó el `home`, borrar el usuario y crearlo nuevamente con las opciones correctas).
21. Crear un grupo `test_group` y agregar el usuario `user_test` a este grupo
22. Verificar en los archivos de configuración del sistema correspondientes si se agregaron el usuario y el grupo recién creados.
23. Crear un directorio `test_data` y allí crear los archivos `a`, `b` y `c`
24. Verificar quién es el `owner` y los permisos correspondientes.
25. Cambiar el `owner` y el `grupo` de los archivos `a` y `b` para que pertenezcan a `test_user` y `test_group`.
26. Para el archivo `a`, darle permisos de lectura y escritura al usuario, solo lectura al grupo y ningun permiso para los otros.
27. Intentar editar el archivo `a` y ver qué sucede.
28. Borrar el usuario `test_user` y el grupo `test_group`
