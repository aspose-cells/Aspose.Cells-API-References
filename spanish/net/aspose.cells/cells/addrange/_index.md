---
title: "Cells.AddRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Añade una referencia de objeto de rango a las celdas"
type: docs
url: /es/net/aspose.cells/cells/addrange/
---
## Cells.AddRange method

Agrega una referencia de objeto de rango a las celdas

```csharp
public void AddRange(Range rangeObject)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rangeObject | Rango | El objeto de rango se contendrá en las celdas |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodAddRangeWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establece algunos datos de muestra en el rango
            cells["A1"].PutValue("A1");
            cells["A2"].PutValue("A2");
            cells["B1"].PutValue("B1");
            cells["B2"].PutValue("B2");

            // Crea un rango y añádelo usando AddRange
            Aspose.Cells.Range range = cells.CreateRange("A1", "B2");
            cells.AddRange(range);

            // Modifica la hoja de cálculo para demostrar la expansión del rango
            cells.InsertRow(1);
            cells.InsertColumn(1);

            Console.WriteLine($"Range now has {range.RowCount} rows and {range.ColumnCount} columns");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


