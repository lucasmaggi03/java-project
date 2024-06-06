# Lenguaje de programación Java
## Ingeniería en Sistema de Información
### Año: 2024

**Profesores:**
- Meca, Adrian
- Tabacman, Ricardo

**Integrantes:**
- Fiorini, Mauricio Mateo. (Leg.: 50475)
- Gil, Agustín. (Leg.: 50412)
- Herrera, Nicolás. (Leg.: 51541)
- Maggi, Lucas Nahuel. (Leg.: 50360)

## 1 - Enunciado

El sistema a desarrollar se tratará de una tienda virtual de ventas de componentes de informática, con ensamble de computadoras y un sistema de órdenes y pedidos, con inicio y registro de usuario con distintos niveles de acceso (administrador, invitado y usuario).

## 2 - Diagrama entidad-relación
![Diagrama entidad-relación](https://i.imgur.com/OCRdaAE.png)

## Checklist

### Regularidad

| Requerimento         | cant. mín. 1 o 2 integ | cant. máx. 3 o 4 integ | Detalle/Listado de casos incluidos |
|----------------------|------------------------|------------------------|-------------------------------------|
| ABMC SIMPLE          | 1 x integ              | 1 x integ              | Categorías, Localidades, Provincias |
| ABMC DEPENDIENTE     | 1                      | 2                      | Componentes, Personas               |
| CUU NO ABMC          | 1                      | 2                      | Registrar Pedidos, Gestión del envío|
| Listado simple       | 1                      | 3*                     | Listado de clientes, Listado de componentes, Listado de pedidos |
| Listado complejo     | 0                      | 1*                     | Listado de componentes por categoría|

### Aprobación directa

| Requerimento         | cant. mín. 1 o 2 integ | cant. máx. 3 o 4 integ | Detalle/Listado de casos incluidos |
|----------------------|------------------------|------------------------|-------------------------------------|
| ABMC                 | todos                  | todos                  | Categorías, Componentes             |
| CU “Complejo” (nivel resumen) | 1           | 2                      | Realizar una venta, Armado de computadora |
| Listado complejo     | 1                      | 2                      | Listado de componentes por categoría, Listado de pedidos por intervalo de fechas |
| Nivel de acceso      | 2                      | 2                      | Usuario, Administrador              |
| Manejo de errores    | obligatorio            | obligatorio            | no requiere detalle                |
| requerimiento extra obligatorio | 0          | 1                      | Envío de email para confirmar registro en la página |
| publicar el sitio    | obligatorio            | obligatorio            | no requiere detalle                |