---
title: "Enumeración SortOrder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.SortOrder enum. Representa el orden de clasificación para el rango de datos"
type: docs
url: /es/net/aspose.cells/sortorder/
---
## SortOrder enumeration

Representa el orden de clasificación para el rango de datos.

```csharp
public enum SortOrder
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Ascending | `0` | Ordena los datos en orden ascendente |
| Descending | `1` | Ordena los datos en orden descendente |
| Natural | `2` | Mantiene el orden original de los datos sin ordenar. Solo se aplica a algunos escenarios especiales como PivotTable. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSortOrderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            var workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para ordenar
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);
            
            // Crear un clasificador de datos
            var sorter = workbook.DataSorter;
            
            // Establecer el orden de clasificación y las claves
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Definir área de ordenación
            var sortArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };
            
            // Ejecuta la ordenación
            sorter.Sort(worksheet.Cells, sortArea);
            
            // Guarda el libro de trabajo
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


