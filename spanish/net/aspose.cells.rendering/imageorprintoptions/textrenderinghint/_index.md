---
title: "ImageOrPrintOptions.TextRenderingHint"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Especifica la calidad del renderizado de texto. El valor predeterminado es TextRenderingHint.SystemDefault"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/textrenderinghint/
---
## ImageOrPrintOptions.TextRenderingHint property

Especifica la calidad del renderizado de texto. El valor predeterminado es TextRenderingHint.SystemDefault

```csharp
public TextRenderingHint TextRenderingHint { get; set; }
```

### Ejemplos

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
            
            // Agregar texto de ejemplo para demostrar el renderizado de texto
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

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


