---
title: "AutoFitterOptions.FormatStrategy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFitterOptions-egenskap. Hämtar och anger den formaterade strategin"
type: docs
url: /sv/net/aspose.cells/autofitteroptions/formatstrategy/
---
## AutoFitterOptions.FormatStrategy property

Hämtar och anger den formaterade strategin.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Anmärkningar

Standardvärdet är CellStyle för prestanda.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in exempeldata och radbryt text
            worksheet.Cells["A1"].PutValue("Sample text for FormatStrategy demo");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Skapa AutoFitterOptions med FormatStrategy
            AutoFitterOptions options = new AutoFitterOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine
            };

            // Tillämpa automatisk anpassning med de angivna alternativen
            worksheet.AutoFitRows(options);

            // Spara resultatet
            workbook.Save("FormatStrategyDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


