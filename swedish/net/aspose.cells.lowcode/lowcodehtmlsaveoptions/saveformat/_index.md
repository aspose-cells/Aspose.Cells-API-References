---
title: "LowCodeHtmlSaveOptions.SaveFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeHtmlSaveOptions egenskap. Hämtar och anger formatet för kalkylbladet"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/
---
## LowCodeHtmlSaveOptions.SaveFormat property

Hämtar och anger formatet för kalkylbladet.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Anmärkningar

När du ändrar denna egenskap kommer det sparformat som anges av [`HtmlOptions`](../htmloptions/) att ignoreras (om det tidigare har angetts).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");

            LowCodeHtmlSaveOptions options = new LowCodeHtmlSaveOptions();
            Console.WriteLine("Current SaveFormat value: " + options.SaveFormat);

            options.SaveFormat = SaveFormat.Html;
            options.HtmlOptions = new HtmlSaveOptions();

            workbook.Save("LowCodeHtmlExport.html", options.HtmlOptions);
        }
    }
}
```

### Se även

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


