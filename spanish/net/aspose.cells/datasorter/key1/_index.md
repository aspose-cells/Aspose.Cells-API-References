---
title: "DataSorter.Key1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorter. Representa el índice de la primera columna ordenada, posición absoluta, la columna A es 0, B es 1"
type: docs
url: /es/net/aspose.cells/datasorter/key1/
---
## DataSorter.Key1 property

Representa el índice de la primera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

```csharp
public int Key1 { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey1Demo
    {
        public static void Run()
        {
            // Crea un libro y añade datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);

            // Crear un data sorter y establecer Key1 para ordenar por la columna Score (columna B)
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 1; // Column index 1 (B)
            sorter.Order1 = SortOrder.Descending;

            // Definir el área de ordenación (filas 1-4, todas las columnas de datos)
            CellArea sortArea = new CellArea();
            sortArea.StartRow = 1;
            sortArea.EndRow = 4;
            sortArea.StartColumn = 0;
            sortArea.EndColumn = cells.MaxDataColumn;

            // Ejecuta la ordenación
            sorter.Sort(cells, sortArea);

            // Guardar el resultado
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Ver también

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


