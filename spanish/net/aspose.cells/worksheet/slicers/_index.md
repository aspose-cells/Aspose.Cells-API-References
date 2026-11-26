---
title: "Worksheet.Slicers"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtenga la colección Slicer en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/slicers/
---
## Worksheet.Slicers property

Obtén la colección de Slicer en la hoja de cálculo

```csharp
public SlicerCollection Slicers { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertySlicersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo para la tabla
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // Agregar una tabla
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Agregar slicers a la hoja de cálculo
            worksheet.Slicers.Add(table, table.ListColumns[0], 1, 3);
            worksheet.Slicers.Add(table, 1, "D1");
            worksheet.Slicers.Add(table, table.ListColumns[0], "G1");

            // Guarda el libro de trabajo
            workbook.Save("SlicersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SlicerCollection](../../../aspose.cells.slicers/slicercollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


