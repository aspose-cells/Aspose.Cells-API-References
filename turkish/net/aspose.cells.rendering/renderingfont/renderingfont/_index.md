---
title: "RenderingFont.RenderingFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingFont yapıcı. RenderingFont'ın yeni bir örneğini başlatır"
type: docs
url: /tr/net/aspose.cells.rendering/renderingfont/renderingfont/
---
## RenderingFont constructor

Yeni bir [`RenderingFont`](../) örneğini başlatır

```csharp
public RenderingFont(string fontName, float fontSize)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontName | String | yazı tipi adı |
| fontSize | Single | yazı tipi boyutu nokta cinsinden |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontMethodCtorWithStringSingleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir yazı tipi oluşturun #ctor(string, single) yapıcıyı kullanarak
            RenderingFont font = new RenderingFont("Arial", 24f);
            font.Bold = true;
            font.Color = System.Drawing.Color.Red;
            
            // Stil oluşturun ve yazı tipini ayarlayın
            Style style = workbook.CreateStyle();
            style.Font.Name = font.Name;
            style.Font.Size = (int)font.Size;  // Explicit cast from float to int
            style.Font.IsBold = font.Bold;
            style.Font.Color = font.Color;
            
            // Stili hücreye uygulayın
            worksheet.Cells["A1"].PutValue("Text with custom font");
            worksheet.Cells["A1"].SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FontDemoOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


