---
title: "AutoFitterOptions.AutoFitMergedCellsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFitterOptions-egenskap. Hämtar och anger typen av automatisk anpassning av radhöjd för sammanslagna celler"
type: docs
url: /sv/net/aspose.cells/autofitteroptions/autofitmergedcellstype/
---
## AutoFitterOptions.AutoFitMergedCellsType property

Hämtar och anger typen av automatisk anpassning av radhöjd för sammanslagna celler.

```csharp
public AutoFitMergedCellsType AutoFitMergedCellsType { get; set; }
```

### Anmärkningar

Excel ignorerar som standard sammanslagna celler när radhöjden anpassas, så Aspose.Cells fungerar som MS Excels standard. Vänligen ange den här typen för att ändra hur radhöjden automatiskt anpassas för sammanslagna celler.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempeldata och slå ihop celler
            worksheet.Cells["A1"].PutValue("This is a sample text for merged cells auto-fit demonstration");
            worksheet.Cells.Merge(0, 0, 3, 2); // Merge A1:B3

            // AutoFit-rader med AutoFitMergedCellsType.EachLine
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // AutoFit-kolumner med AutoFitMergedCellsType.EachLine
            worksheet.AutoFitColumns(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Spara arbetsboken
            workbook.Save("AutoFitMergedCellsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [AutoFitMergedCellsType](../../autofitmergedcellstype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


