---
title: "ImageOrPrintOptions.TextRenderingHint"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Указывает качество отображения текста. Значение по умолчанию — TextRenderingHint.SystemDefault"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/textrenderinghint/
---
## ImageOrPrintOptions.TextRenderingHint property

Указывает качество рендеринга текста. Значение по умолчанию — TextRenderingHint.SystemDefault

```csharp
public TextRenderingHint TextRenderingHint { get; set; }
```

### Примеры

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
            
            // Добавьте пример текста для демонстрации отображения текста
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

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


