---
title: "Enumeración GridLoadDataFilterOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.GridDesktop.Data.GridLoadDataFilterOptions. Representa las opciones para filtrar datos al cargar el libro de trabajo desde una plantilla"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridloaddatafilteroptions/
---
## GridLoadDataFilterOptions enumeration

Representa las opciones para filtrar datos al cargar el libro de trabajo desde una plantilla.

```csharp
public enum GridLoadDataFilterOptions
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| All | `2147483647` | Cargar todo |
| CellBlank | `1` | Cargar celdas cuyo valor está vacío |
| CellString | `2` | Cargar celdas cuyo valor es una cadena |
| CellNumeric | `4` | Cargar celdas cuyo valor es numérico (incluyendo fecha y hora) |
| CellError | `8` | Cargar celdas cuyo valor es error |
| CellBool | `16` | Cargar celdas cuyo valor es booleano |
| CellValue | `31` | Cargar solo el valor de las celdas (todos los tipos de valor) |
| Formula | `32` | Cargar fórmulas de celdas. |
| CellData | `67108927` | Cargar datos de celdas incluyendo valores, fórmulas y formato |
| Chart | `256` | Cargar gráficos |
| Drawing | `402653952` | Objetos de dibujo (incluyendo Gráfico, Imagen, OleObject y todos los demás objetos de dibujo) |
| MergedArea | `1024` | Cargar celdas combinadas |
| ConditionalFormatting | `2048` | Cargar formato condicional |
| DataValidation | `4096` | Cargar validaciones de datos |
| PivotTable | `8192` | Cargar tablas dinámicas |
| Table | `16384` | Cargar tablas |
| Hyperlinks | `32768` | Cargar hipervínculos |
| SheetSettings | `65536` | Cargar configuraciones de la hoja de cálculo |
| SheetData | `403701759` | Cargar todos los datos de la hoja de cálculo, como datos de celdas, configuraciones, objetos, ...etc. |
| BookSettings | `1048576` | Cargar configuraciones del libro |
| Settings | `1114112` | Cargar configuraciones del libro y de la hoja de cálculo |
| XmlMap | `2097152` | Cargar XmlMap |
| Structure | `4194304` | Cargar estructura del libro |
| DocumentProperties | `8388608` | Cargar propiedades del documento |
| DefinedNames | `16777216` | Cargar objetos de nombres definidos |
| VBA | `33554432` | Cargar proyectos VBA |
| Style | `67108864` | Cargar estilos para el formato de celdas |
| Picture | `134217728` | Cargar imágenes |
| OleObject | `268435456` | Cargar OleObjects |
| Revision | `536870912` | Cargar registros de revisiones |

### Ver también

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


