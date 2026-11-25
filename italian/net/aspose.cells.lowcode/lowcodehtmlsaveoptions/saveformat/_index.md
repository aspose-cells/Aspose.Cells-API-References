---
title: "LowCodeHtmlSaveOptions.SaveFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "LowCodeHtmlSaveOptions proprietà. Ottiene e imposta il formato del foglio di calcolo"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/
---
## LowCodeHtmlSaveOptions.SaveFormat property

Ottiene e imposta il formato del foglio di calcolo.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Osservazioni

Quando si modifica questa proprietà, il formato di salvataggio specificato da [`HtmlOptions`](../htmloptions/) verrà ignorato (se era stato specificato in precedenza).

### Esempi

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

### Vedi anche

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


