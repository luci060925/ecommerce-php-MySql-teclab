# eCommerce Teclab

> PHP + MySQL product catalog with MVC-inspired architecture, PDO prepared statements, and AJAX dynamic loading.

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

> Proyecto final — Teclab, Tecnicatura Superior en Programación (2026).

## Sobre el proyecto

Catálogo de productos de hardware construido con PHP y MySQL, organizado por categorías y renderizado dinámicamente. Usa PDO con prepared statements en todo el proyecto y una estructura modular inspirada en MVC.

## Funcionalidades

- **Catálogo de productos** — listado dinámico de hardware (CPU, GPU, RAM, etc.).
- **Categorías** — productos vinculados por `categoria_id`.
- **OOP** — clases reutilizables, separación de responsabilidades.
- **Consulta con JOIN** — productos + nombre de categoría en una sola query (`LEFT JOIN`).
- **AJAX** — carga dinámica de contenido sin recargas de página.
- **UI responsive** — funciona en móvil y escritorio.

## Estructura

```
ecommerce-php-MySql-teclab/
├── index.php        Router principal
├── /assets          Estilos CSS + imágenes de productos
├── /backend         Handlers PHP para peticiones AJAX
├── /class           Clases principales (database, productos, categorias, autoload)
└── /views           Templates del frontend
```

## Instalación

**Requisitos:** PHP 8.x, MySQL 5.7+/8.x, Apache (XAMPP/Laragon).

```bash
git clone https://github.com/luci060925/ecommerce-php-MySql-teclab.git
```

1. Crear base de datos MySQL llamada `miproyecto`.
2. Importar el esquema:
   ```bash
   mysql -u root -p miproyecto < miproyecto.sql
   ```
3. Verificar la configuración en `class/database.php` (por defecto: `host=localhost`, `user=root`, sin contraseña — compatible con XAMPP estándar).
4. Abrir `http://localhost/ecommerce-php-MySql-teclab/`.

---

**Luciana Mansilla** · [LinkedIn](https://www.linkedin.com/in/luciana-mansilla-854bb5419/) · [GitHub](https://github.com/luci060925)
