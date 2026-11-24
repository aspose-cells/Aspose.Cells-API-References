---
title: "LowCodeHtmlSaveOptions.SaveFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeHtmlSaveOptions Eigenschaft. Ruft das Format der Tabelle ab und legt es fest"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/
---
## LowCodeHtmlSaveOptions.SaveFormat property

Ermittelt und legt das Format der Tabellenkalkulation fest.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Hinweise

Beim Ändern dieser Eigenschaft wird das von [`HtmlOptions`](../htmloptions/) angegebene Speicherformat ignoriert (falls es zuvor angegeben wurde).

### Beispiele

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

### Siehe auch

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


