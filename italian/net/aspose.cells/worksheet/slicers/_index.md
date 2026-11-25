---
title: "Worksheet.Slicers"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottieni la raccolta di Slicer nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/slicers/
---
## Worksheet.Slicers property

Ottieni la collezione di Slicer nel foglio di lavoro

```csharp
public SlicerCollection Slicers { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi una tabella
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Aggiungi slicer al foglio di lavoro
            worksheet.Slicers.Add(table, table.ListColumns[0], 1, 3);
            worksheet.Slicers.Add(table, 1, "D1");
            worksheet.Slicers.Add(table, table.ListColumns[0], "G1");

            // Salva la cartella di lavoro
            workbook.Save("SlicersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SlicerCollection](../../../aspose.cells.slicers/slicercollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


