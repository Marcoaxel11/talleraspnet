========================================
 INSTRUCCIONES PARA ABRIR EL PROYECTO 
         TALLER ASP.NET CORE
========================================

1. Clonar el repositorio
------------------------
Si no tienes el proyecto en tu PC:
    git clone https://github.com/Marcoaxel11/talleraspnet.git
    cd talleraspnet

Si ya lo tienes, solo actualiza:
    git pull


2. Abrir el proyecto
---------------------
Opción A: Visual Studio
    - Abrir Visual Studio
    - File -> Open -> Project/Solution
    - Seleccionar el archivo: Taller_ASP.NET_Core.sln

Opción B: Visual Studio Code
    - Abrir terminal en la carpeta del proyecto
    - Ejecutar: code .


3. Configurar la base de datos
-------------------------------
El proyecto usa SQLite, no requiere SQL Server.

Verificar que exista el archivo:
    appsettings.json

En appsettings.json debe estar:
    {
      "ConnectionStrings": {
        "DefaultConnection": "Data Source=TareasDB.db"
      }
    }


4. Crear la base de datos (si es necesario)
-------------------------------------------
Si es la primera vez o si borraste la BD:
    dotnet ef database update


5. Ejecutar la aplicación
-------------------------
En terminal:
    dotnet run

En Visual Studio:
    Presionar el botón Start (Iniciar)


6. Abrir en el navegador
------------------------
Ingresar a uno de los siguientes enlaces (el que muestre Visual Studio):

    https://localhost:7017
    http://localhost:5025


NOTA:
-----
Si aparece algún error durante la ejecución, anótalo o toma captura
y te digo cómo solucionarlo.

Estructura del proyecto
/ProyectoTareas
│
├── Controllers/
│   ├── AccountController.cs
│   ├── HomeController.cs
│   ├── TareasController.cs
│
├── Data/
│   ├── ApplicationDbContext.cs
│   ├── SeedData.cs
│
├── Models/
│   ├── Tarea.cs
│   ├── Usuario.cs
│
├── Migrations/
│   └── (Archivos generados automáticamente)
│
├── Views/
│   ├── Account/
│   │   ├── Login.cshtml
│   │   ├── Register.cshtml
│   │
│   ├── Home/
│   │   ├── Index.cshtml
│   │
│   ├── Tareas/
│       ├── Index.cshtml
│       ├── Create.cshtml
│       ├── Edit.cshtml
│       ├── Details.cshtml
│       ├── Delete.cshtml
│
├── wwwroot/
│   ├── css/
│   ├── js/
│   ├── lib/ (Bootstrap, jQuery, etc.)
│
├── appsettings.json
├── Program.cs
├── ProyectoTareas.csproj

credenciales de demostracion:
ejemplo@correo.com
Ejemplo-01
