---
title: "Cells.LastCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskapen. Hämtar den sista cellen i detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/cells/lastcell/
---
## Cells.LastCell property

Hämtar den sista cellen i detta kalkylblad.

```csharp
public Cell LastCell { get; }
```

### Anmärkningar

Returnerar null om det inte finns någon data i kalkylbladet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyLastCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data
            worksheet.Cells["A1"].Value = "Header1";
            worksheet.Cells["B1"].Value = "Header2";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["B2"].Value = "Data2";

            // Hämta den sista cellens adress
            Cell lastCell = worksheet.Cells.LastCell;
            Console.WriteLine("Last cell address: " + lastCell.Name);

            // Skapa ett område från första till sista cellen
            Aspose.Cells.Range fullRange = worksheet.Cells.CreateRange(
                worksheet.Cells.FirstCell.Name, 
                lastCell.Name);
            
            // Tillämpa formatering på området
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            fullRange.ApplyStyle(style, new StyleFlag { FontBold = true });

            // Spara arbetsboken
            workbook.Save("LastCellDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


