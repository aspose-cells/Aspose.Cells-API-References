---
title: "Klass DataBarBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataBarBorder klass. Representerar kanten på datastaplarna som specificeras av en villkorsstyrd formateringsregel"
type: docs
url: /sv/net/aspose.cells/databarborder/
---
## DataBarBorder class

Representerar kanten på datastaplarna som specificeras av en villkorsstyrd formateringsregel.

```csharp
public class DataBarBorder
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Color](../../aspose.cells/databarborder/color/) { get; set; } | Hämtar eller anger kantens färg på datastaplarna som specificeras av en villkorsstyrd formateringsregel. |
| [Type](../../aspose.cells/databarborder/type/) { get; set; } | Hämtar eller anger kantens typ på datastaplarna som specificeras av en villkorsstyrd formateringsregel. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarBorderDemo
    {
        public static void DataBarBorderExample()
        {
            // Skapar en ny arbetsbok
            Workbook workbook = new Workbook();
            // Åtkomst till det första kalkylbladet i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(80);
            worksheet.Cells["A4"].PutValue(60);
            worksheet.Cells["A5"].PutValue(30);

            // Lägger till en tom villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Definierar ett cellområde för villkorsstyrd formatering
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Lägger till ett villkor av typen DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition formatCondition = fcs[conditionIndex];

            // Åtkomst till DataBar
            DataBar dataBar = formatCondition.DataBar;

            // Ställer in DataBar-egenskaperna
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 0;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MaxCfvo.Value = 100;
            dataBar.ShowValue = true;

            // Åtkomst till och inställning av DataBarBorder-egenskaperna
            DataBarBorder dataBarBorder = dataBar.BarBorder;
            dataBarBorder.Type = DataBarBorderType.Solid;
            dataBarBorder.Color = Color.Black;

            // Sparar Excel-filen
            workbook.Save("DataBarBorderExample.xlsx");
            workbook.Save("DataBarBorderExample.pdf");

            Console.WriteLine("DataBar border example created successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


