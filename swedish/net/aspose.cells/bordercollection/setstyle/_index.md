---
title: "BorderCollection.SetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BorderCollection-metod. Ställer in stilen för alla borders i samlingen"
type: docs
url: /sv/net/aspose.cells/bordercollection/setstyle/
---
## BorderCollection.SetStyle method

Anger style för alla kanter i samlingen.

```csharp
public void SetStyle(CellBorderType style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | CellBorderType | Borders stil |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetStyleWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta cell C6 och dess stil
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();

            // Ange border-färg och stil
            style.Borders.SetColor(System.Drawing.Color.Red);
            style.Borders.SetStyle(CellBorderType.Thick);

            // Tillämpa stilen på cellen
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("BorderCollectionMethodSetStyleWithCellBorderTypeDemo_out.xlsx");

            Console.WriteLine("Border style set successfully.");
        }
    }
}
```

### Se även

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


