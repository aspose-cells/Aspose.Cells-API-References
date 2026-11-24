---
title: "FindOptions.SetRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions-Methode. Legt den zu durchsuchenden Bereich fest"
type: docs
url: /de/net/aspose.cells/findoptions/setrange/
---
## FindOptions.SetRange method

Setzt den zu suchenden Bereich.

```csharp
public void SetRange(CellArea ca)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | CellArea | der zu durchsuchende Bereich. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsMethodSetRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Daten befüllen
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("def");
            worksheet.Cells["C3"].PutValue("abc");
            
            // FindOptions erstellen und den Suchbereich festlegen
            FindOptions rangeOptions = new FindOptions();
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 1;
            cellarea.StartColumn = 1;
            cellarea.EndRow = 3;
            cellarea.EndColumn = 3;
            rangeOptions.SetRange(cellarea);
            
            // Im angegebenen Bereich suchen
            rangeOptions.SearchBackward = false;
            Cell foundCell = worksheet.Cells.Find("abc", null, rangeOptions);
            
            Console.WriteLine("Found 'abc' at row: " + foundCell.Row + ", column: " + foundCell.Column);
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


