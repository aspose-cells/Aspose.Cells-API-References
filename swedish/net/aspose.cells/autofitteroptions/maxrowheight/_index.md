---
title: "AutoFitterOptions.MaxRowHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFitterOptions-egenskap. Hämtar och anger maximal radhöjd i enheten Point när rader automatiskt anpassas"
type: docs
url: /sv/net/aspose.cells/autofitteroptions/maxrowheight/
---
## AutoFitterOptions.MaxRowHeight property

Hämtar och anger maximal radhöjd (i enheten Point) vid automatisk anpassning av rader.

```csharp
public double MaxRowHeight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyMaxRowHeightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempeldata och formatering.
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row auto-fitting");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells.SetRowHeight(0, 10); // Set initial small row height

            // Skapa AutoFitterOptions med MaxRowHeight-inställning
            AutoFitterOptions options = new AutoFitterOptions
            {
                MaxRowHeight = 50, // Limit maximum row height to 50 pixels
                OnlyAuto = true
            };

            // Autoanpassa raden med höjdbegränsning
            worksheet.AutoFitRows(0, 0, options);

            Console.WriteLine("Row height after auto-fit with MaxRowHeight=50: " + worksheet.Cells.GetRowHeight(0));

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


