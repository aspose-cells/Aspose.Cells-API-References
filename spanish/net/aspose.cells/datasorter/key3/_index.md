---
title: "DataSorter.Key3"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "DataSorter property. Representa el índice de la tercera columna ordenada posición absoluta la columna A es 0 B es 1"
type: docs
url: /es/net/aspose.cells/datasorter/key3/
---
## DataSorter.Key3 property

Representa el índice de la tercera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

```csharp
public int Key3 { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey3Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["C1"].PutValue("Grade");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["C2"].PutValue("B");
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["C3"].PutValue("A");
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);
            cells["C4"].PutValue("C");
            cells["A5"].PutValue("Eve");
            cells["B5"].PutValue(92);
            cells["C5"].PutValue("A");

            // Crear un clasificador de datos
            DataSorter sorter = workbook.DataSorter;
            
            // Ordenar por Puntuación (descendente), luego por Nombre (ascendente), luego por Calificación (descendente)
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Column B (Score)
            
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 0; // Column A (Name)
            
            sorter.Order3 = SortOrder.Descending;
            sorter.Key3 = 2; // Column C (Grade)
            
            // Ordenar el rango de datos
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 5, 2));

            // Guarda el libro de trabajo
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Ver también

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


