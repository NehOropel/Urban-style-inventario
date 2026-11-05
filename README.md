# Urban Style · Módulo de Inventario y Stock

> Trabajo Práctico Integrador y Progresivo (TPI) · Organización Empresarial
> Tecnicatura Universitaria en Programación · Universidad Tecnológica Nacional (UTN)

## Descripción del sistema

**Urban Style** es una tienda de indumentaria y accesorios (empresa ficticia) con local físico y tienda online.
Este proyecto propone un **módulo de gestión de inventario y stock** que:

- registra los productos por **talle y color** (la unidad real de stock es la variante);
- **descuenta el stock automáticamente** cuando se concreta una venta (local u online);
- registra **entradas de mercadería, devoluciones y ajustes**;
- genera **alertas de stock mínimo** para el área de Compras;
- produce **reportes de inventario** para la administración.

El módulo se relaciona con las áreas de Ventas, Compras, Depósito y Administración, y con los proveedores.

**Objetivo general:** desarrollar e implementar, en 21 semanas, el módulo de inventario y stock de Urban Style para reducir los faltantes de mercadería y brindar información confiable para la toma de decisiones.

## Integrantes

| Integrante | Rol en el proyecto |
|---|---|
| Oropel Zabaleta, Nehuen Alejandro | Creador del proyecto |


## Documentación técnica

| Documento | Descripción |
|---|---|
| [`docs/bpmn-reposicion-stock.png`](docs/bpmn-reposicion-stock.png) | Diagrama BPMN del proceso de venta con control de stock y reposición |
| [`docs/historias-de-usuario.md`](docs/historias-de-usuario.md) | Backlog: tres historias de usuario con criterios de aceptación |
| [`docs/indicadores-de-control.md`](docs/indicadores-de-control.md) | Indicadores de control y estándares de desempeño |
| `docs/entregas/` | Entregas 1 a 3 del TPI en PDF (sistema abierto, FODA y Gantt, organigrama y diccionario de datos) |

## Proceso modelado (BPMN)

![Proceso BPMN: venta con control de stock y reposición](docs/bpmn-reposicion-stock.png)

El diagrama usa Pools (Cliente, Urban Style, Proveedor) y Lanes (Vendedor, Sistema, Compras, Depósito), con tres compuertas exclusivas para las excepciones: sin stock, stock en nivel mínimo y mercadería no conforme.

## Gestión del backlog

Tablero: [COMPLETAR: URL del tablero de GitHub Projects]

Columnas: **Por Hacer → En Progreso → Listo**. Cada historia de usuario es un *issue* vinculado a su Pull Request.

## Flujo de trabajo con Git

- `main`: rama estable. **No se hacen commits directos**; todo ingresa por Pull Request.
- Ramas secundarias con el formato `tipo/descripcion-corta` (por ejemplo `docs/bpmn-reposicion-stock`).
- Mensajes de commit con el formato `tipo: descripción en presente` (`docs`, `feat`, `fix`, `chore`, `test`).
- Cada Pull Request requiere **al menos una revisión de un par** antes de fusionarse.

## Declaración de uso de IA

> Esta sección declara qué asistente de IA se usó, con qué prompts y qué correcciones humanas se hicieron. Es responsabilidad del equipo: la IA no exime de la veracidad y coherencia del trabajo.

**Asistente utilizado:** Claude (Anthropic).

**Propósitos:** estructurar las entregas, proponer borradores (FODA, metas, Gantt, organigrama, diccionario de datos, BPMN, historias de usuario, indicadores) y dar formato a los documentos.

### Prompts utilizados y justificación

| N.º | Prompt (resumen) | Por qué se usó |
|---|---|---|
| 1 | Se pidió estructurar organigrama y diccionario de datos. | Obtener un primer borrador a revisar. |
| 2 | Se pidió estructurar BPMN, historias de usuario, indicadores y este README. | Tener una base para auditar y corregir. |

### Correcciones humanas sobre los resultados de la IA

| Qué propuso la IA | 
|---|---|---|
| Roles y plazos del Gantt. |
| Estructura del organigrama y entidades del diccionario. | 
| Flujo BPMN y compuertas. | 
| Historias de usuario y criterios de aceptación. |

> Limitaciones reconocidas: la IA puede inventar datos o cometer errores conceptuales. Todo contenido fue revisado por el equipo, que responde por él.
