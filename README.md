# 🛍️  Gestión de Artículos

Este proyecto corresponde a un Trabajo Práctico de Programación en C# con Windows Forms (WinForms).
Se trata de una aplicación de escritorio para la gestión de artículos de un catálogo de un comercio, con el objetivo de mantener la información organizada y lista para ser consumida por distintos servicios (web, e-commerce, apps móviles, revistas, etc.).

### 📌 Funcionalidades principales

La aplicación permite administrar artículos mediante operaciones básicas de lectura, creación, modificación y eliminación:

✅ Listado de artículos.

🔍 Búsqueda de artículos por distintos criterios.

➕ Alta de artículos.

✏️ Modificación de artículos.

🗑️ Eliminación de artículos.

👁️ Ver detalle completo de un artículo.

#### Además:

Administración de Marcas y Categorías.

Posibilidad de asignar una o más imágenes a cada producto, sin límite establecido.

Persistencia de los datos en una base de datos SQL Server (provista previamente).

### 📦 Datos mínimos de un artículo

Cada artículo deberá contar con la siguiente información:

- Código de artículo

- Nombre

- Descripción

- Marca (seleccionable de una lista desplegable)

- Categoría (seleccionable de una lista desplegable)

- Imagen (una o varias)

- Precio

### ⚙️ Tecnologías utilizadas

- Lenguaje: C#

- Framework: .NET Framework / WinForms

- Base de datos: SQL Server

- ORM / Acceso a datos: ADO.NET / SQL nativo

- IDE recomendado: Visual Studio



## 📂 Estructura del proyecto



#### 🖼 Capa de Presentación (UI / Formularios)



📌 Acá van todos los WinForms que interactúan con el usuario.

- Form1 → Catalogo de articulos con listado completo

- SplashScreen → Pantalla de carga inicial.

- frmMenuPrincipal → Menú central con navegación al resto de formularios.

- AgregarArticulo → Form para registrar/editar artículos.

- AgregarCategoria → Form para registrar categorías.

- AgregarMarca → Form para registrar marcas.

- frmCategorias → Listado/gestión de categorías.

- frmMarcas → Listado/gestión de marcas.



#### 🧩 Capa de Dominio (Entidades / Modelos)


- Articulo → Atributos como Id, Nombre, Código Descripcion, Precio, Categoria, Marca, List<Imagen>.

- Categoria → Atributos como Id, Descripcion.

- Marca → Atributos como Id, Descripcion.

- Imagen → Atributos como Id, Url e IdArticulo (para asociar imágenes a artículos).



#### 🏗 Capa de Negocio (Reglas y Acceso a Datos)


 📌 Clases que contienen la lógica de negocio y comunicación con la base de datos.

- AccesoDatos
👉 Clase de utilidad para manejar conexiones, consultas (SqlConnection, SqlCommand, etc.).
⚡ Ejemplo: abrir conexión, ejecutar SELECT, INSERT, UPDATE, DELETE.

- ArticuloNegocio
👉 Métodos como listar(), agregarArticulo , modificarArticulo, eliminarArticulo.

- CategoriaNegocio
👉 Atla/Baja de categorías.

- MarcaNegocio
👉 Atla/Baja  de marcas.

- ImagenNegocio
👉 Manejo de imágenes (asociar, listar, eliminar).




## 👨‍💻 Autores

- Mateo Leon Maciel
