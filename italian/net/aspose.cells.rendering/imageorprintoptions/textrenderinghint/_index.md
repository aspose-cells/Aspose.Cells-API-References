---
title: "ImageOrPrintOptions.TextRenderingHint"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Specifica la qualità del rendering del testo. Il valore predefinito è TextRenderingHint.SystemDefault"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/textrenderinghint/
---
## ImageOrPrintOptions.TextRenderingHint property

Specifica la qualità del rendering del testo. Il valore predefinito è TextRenderingHint.SystemDefault

```csharp
public TextRenderingHint TextRenderingHint { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTextRenderingHintDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi testo di esempio per dimostrare il rendering del testo
            worksheet.Cells["A1"].PutValue("Text Rendering Hint Demo");
            
            HtmlSaveOptions options = new HtmlSaveOptions();
#if !NETCOREAPP3_1_OR_GREATER
            options.ImageOptions.TextRenderingHint = TextRenderingHint.AntiAlias;
#endif
            workbook.Save("output.html", options);
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


