---
title: "AccessCacheOptions Enumeración"
linktitle: "AccessCacheOptions"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Enumeración AccessCacheOptions. Encapsula el objeto que representa accesscacheoptions en Go."
type: docs
weight: 200
url: /es/go-cpp/accesscacheoptions/
---

## AccessCacheOptions Enum

Opciones de caché para el acceso a datos. Se pueden combinar múltiples opciones usando el operador "|".

```go

type AccessCacheOptions int32


```

## Fields

| Field | Description |
| --- | --- |
| [None](./none/) | Sin caché para ningún acceso a datos. |
| [All](./all/) | Aplicar todas las optimizaciones posibles para todo tipo de acceso a datos en el workbook. No se deben cambiar los ajustes y datos durante el acceso optimizado. |
| [PositionAndSize](./positionandsize/) | Aplicar optimización posible para obtener la posición y el tamaño del objeto (por ejemplo, Shape). No se deben cambiar los ajustes de altura de fila y ancho de columna durante el acceso optimizado. |
| [CellsData](./cellsdata/) | Aplicar optimización posible para obtener los valores de las celdas. Los datos de las celdas (datos y configuraciones de Cell, Row) no deben cambiarse durante el acceso optimizado, tampoco deben crearse nuevos objetos Cell/Row (por ejemplo, mediante <see cref=\"Cells.this[int, int]\"/>). |
| [CellDisplay](./celldisplay/) | Aplicar optimización posible para obtener resultados relacionados con la visualización de celdas (<see cref=\"Cell.DisplayStringValue\"/>, <see cref=\"Cell.GetStyle()\"/>, <see cref=\"Cell.GetDisplayStyle()\"/>, etc.). Los datos de las celdas y los objetos relacionados con el estilo (estilos de Cell/Row/Column, ancho de columna, etc.) no deben cambiarse durante el acceso optimizado. |
| [GetFormula](./getformula/) | Aplicar optimización posible para obtener fórmulas. Todos los datos y configuraciones que puedan afectar la expresión de la fórmula (nombre del Worksheet, texto del Name, columna de la tabla, etc.) no deben cambiarse durante el acceso optimizado. |
| [SetFormula](./setformula/) | Aplicar optimización posible para establecer fórmulas. Todos los datos y configuraciones que puedan afectar la expresión de la fórmula (nombre del Worksheet, texto del Name, columna de la tabla, etc.) no deben cambiarse durante el acceso optimizado. |
| [CalculateFormula](./calculateformula/) | Aplicar optimización posible para calcular fórmulas. Los datos de las celdas no deben cambiarse durante el acceso optimizado, tampoco deben crearse nuevos objetos (Cell, Row, etc.) (por ejemplo, mediante <see cref=\"Cells.this[int, int]\"/>). |
| [ConditionalFormatting](./conditionalformatting/) | Aplicar optimización posible para obtener el resultado de formato de los formateos condicionales. Todos los datos y configuraciones que puedan afectar el resultado de los formateos condicionales (configuraciones de los formateos condicionales, valores de celdas dependientes, etc.) no deben cambiarse durante el acceso optimizado. |
| [Validation](./validation/) | Aplicar optimización posible para obtener el resultado de la validación. Todos los datos y configuraciones que puedan afectar el resultado de la validación (configuraciones de la validación, valores de celdas dependientes, etc.) no deben cambiarse durante el acceso optimizado. |
