##  Descripción del Proyecto
Este proyecto consiste en el desarrollo de una plataforma web de recetas saludables, enfocada en promover una alimentación equilibrada, accesible y consciente para todo tipo de usuarios.
El sitio está alineado con el bienestar y la salud nutricional, ofreciendo recetas fáciles de preparar y adaptadas a distintas necesidades alimenticias, como dietas vegetarianas, veganas, sin gluten o bajas en calorías. Además, la plataforma busca educar a los usuarios sobre los beneficios de mantener hábitos alimenticios saludables.

## Objetivo General
Desarrollar una plataforma web que permita a los usuarios descubrir, organizar y aprender sobre recetas saludables, fomentando una mejor calidad de vida a través de la nutrición.

## Objetivos Específicos

- Facilitar la búsqueda de recetas según ingredientes, tipo de dieta o tiempo de preparación.-

- Permitir a los usuarios guardar recetas favoritas y crear listas de compras.-

- Brindar información nutricional y consejos prácticos sobre alimentación saludable.-
  
- Ofrecer una interfaz intuitiva, moderna y adaptable a dispositivos móviles.- 


# Características Claves del Sitio
## Buscador de Recetas
Permite buscar recetas de forma rápida y sencilla utilizando filtros como:
- Ingredientes-
- Tipo de dieta-
- Tiempo de preparación-

## Consejos Nutricionales
Sección dedicada a:
- Artículos sobre alimentación saludable
- Recomendaciones nutricionales
- Educación sobre hábitos alimenticios positivos

## Interfaz Amigable
- Diseño intuitivo y fácil de usar
- Adaptable a dispositivos móviles (responsive design)
- Enfocada en la experiencia del usuario
- 
# Arquitectura del Sitio
## Página Principal
- Presentación general del sitio
- Acceso rápido a las secciones principales
## Página de Recetas
- Listado de recetas disponibles
- Filtros de búsqueda
## Detalles de Receta
- Ingredientes
- Pasos de preparación
- Información adicional

### Funcionalidades Clave

1. **Gestión de Clientes**  
- Agregar, editar o eliminar clientes.
- Campos: nombre, edad, contacto, ID único y tipo de membresía asignada.
- Opción de actualizar y modificar la información del usuario.
2. **Asignación de Membresías**
- Tres tipos predefinidos: mensual, trimestral y anual.
- Cada tipo tiene un precio fijo almacenado en la tabla membresias.
- Al seleccionar una membresía, el precio se carga automáticamente

3. **Buscador de Clientes**  
- Localiza usuarios rápidamente por nombre o ID.
- Muestra su membresía y precio asociado.

4. **Actualización Automática**  
  - Todos los cambios se reflejan en tiempo real en la base de datos MySQL.
## Impacto de Funcionalidades:
Con esta implementación, los gimnasios podrán gestionar de manera eficiente la información de sus clientes y ofrecer la opción de elegir áreas de entrenamiento de manera organizada. La digitalización del registro mejorará la administración interna y la satisfacción de los clientes al brindarles una plataforma accesible y funcional.

## Modelo relacion en MYSQL
**Tablas Principales**
1. **Clientes**
- id_cliente (PK)
- nombre
- edad
- contacto
- id_membresia (FK)
2. **membresias**
-  tipo (Mensual, Trimestral, Anual) (PK)
-  precio

![Image1](https://github.com/luxmzl/appStartFit/blob/main/ModeloRelacionalGimnasio.png)

## Tablas Principales
1. **Clientes**: Esta tabla almacena la información personal de los clientes del gimnasio, incluyendo sus datos de contacto.
2. **Membresía**: Esta tabla contiene los planes de membresía adquiridos por los clientes.

## Script del modelo físico: Archivo SQL con las sentencias para crear las tablas y relaciones en MySQL. 
![Image2](https://github.com/luxmzl/appStartFit/blob/main/script.png)


[Abrir el script](https://github.com/luxmzl/appGymHub/blob/main/EXAMEN%20ABP%20GYMHUB%20(1).sql)
