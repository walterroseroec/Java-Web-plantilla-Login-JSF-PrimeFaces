
# Java Web plantilla de Login con JSF y PrimeFaces

Este proyecto es una plantilla básica para aplicaciones web desarrolladas con JSF y PrimeFaces. Incluye una implementación inicial con páginas comunes como un formulario de inicio de sesión, una página de inicio, y páginas de error personalizadas para códigos 403 y 404.

## Características

- **Login:** Página de inicio de sesión para la autenticación de usuarios.
- **Home:** Página principal para redirigir al usuario autenticado.
- **Errores personalizados:** Páginas diseñadas para manejar errores 403 (Prohibido) y 404 (No encontrado).
- **Estilos modernos:** Uso de PrimeFlex CSS para diseño responsivo y PrimeIcons para íconos.

## Tecnologías

- **Java Web**
- **JSF (Jakarta Server Faces)**
- **PrimeFaces 12 o superior**
- **PrimeFlex  v3 CSS**
- **PrimeIcons v7 CSS**

## Estructura del proyecto
Puedes asignar los recursos a tu manera, aun así te dejo la estructura más utilizada con servidores de aplicaciones.
```
src/main/webapp/
├── resources/
│   ├── css/
│   │   ├── primeflex.min.css
│   │   └── primeicons.css
│   ├── icons/
│   │   └── ..
│   └── ...
├── login.xhtml
├── home.xhtml
├── 403.xhtml
└── 404.xhtml
```
Pero si usas JoinFaces esta es la estructura más utilizada.
```
src/main/webapp/
├── assets/
│   ├── css/
│   │   ├── primeflex.min.css
│   │   └── primeicons.css
│   ├── icons/
│   │   └── ..
│   └── ...
├── login.xhtml
├── home.xhtml
├── 403.xhtml
└── 404.xhtml
```
Considera lo siguiente: dentro del archivo de primeicons.css existen rutas asignadas de la siguiente forma **"#{resource['assets:icons/primeicons.eot']}"**, recomendamos que el nombre de **assets** lo reemplaces si no usas JoinFaces por **resources** para que no tengas inconvenientes al leer las fuentes de los iconos.
## Requisitos previos

- JDK 11 o superior
- Servidor de aplicaciones compatible con Jakarta EE (WildFly, Payara, TomEE, etc.)
- Maven 3.6+

## Personalización

Puedes modificar las páginas `.xhtml` y los recursos CSS según las necesidades de tu proyecto.

## Contribuciones

¡Las contribuciones son bienvenidas! Si tienes ideas para mejorar este proyecto, siéntete libre de abrir un issue o enviar un pull request.

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.
