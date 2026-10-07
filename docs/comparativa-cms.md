# Comparativa de gestores de contenidos

| | Joomla | Drupal |
|---|---|---|
| Tipo de sitio para el que sirve | Webs corporativas, blogs, portales medianos y comunidades; equilibrio entre facilidad y potencia | Portales grandes y complejos, con mucho contenido estructurado, usuarios con distintos permisos y alta escalabilidad |
| Licencia | GPL v2 o posterior (software libre) | GPL v2 o posterior (software libre) |
| Tiempo hasta ver la portada | Unos 8 minutos (incluye la espera del arranque de MariaDB) | Unos 5 minutos |
| Dificultad del instalador (1-5) | 2 (fácil, pero hay que introducir los datos de la base de datos) | 2 (fácil, con SQLite no hay que configurar nada de BD) |
| Base de datos que usa | MariaDB/MySQL (en la práctica, MariaDB 11 en un contenedor aparte; también admite PostgreSQL) | SQLite en la práctica (sin servidor aparte); también admite MySQL/MariaDB y PostgreSQL |
| Imagen de Docker Hub | joomla | drupal |

## ¿Qué gestor elegirías para cada caso y por qué?

1. **El blog de un club deportivo:** Joomla. Es sencillo de instalar y de manejar para gente sin perfil técnico, y para un blog con noticias, resultados y galerías sobra con lo que trae de serie. Drupal sería excesivo para este caso.

2. **La web de una universidad, con muchos tipos de contenido:** Drupal. Permite definir tipos de contenido propios (grados, asignaturas, profesores, noticias, eventos), relacionarlos con taxonomías y controlar con detalle roles y permisos (departamentos, editores, administradores). Escala bien con mucho contenido y tráfico, aunque tiene una curva de aprendizaje mayor.

3. **Una revista con secciones en varios idiomas:** Joomla. Trae el multidioma integrado en el núcleo y es fácil enlazar cada artículo con sus traducciones, además de organizar el contenido por categorías/secciones. Drupal también lo hace muy bien y es más potente, pero para una revista la rapidez de configuración de Joomla compensa.
