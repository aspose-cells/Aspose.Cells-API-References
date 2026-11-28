---
title: "Shape.HtmlText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Bu metin kutusunda veri ve bazı biçimlendirmeleri içeren html dizesini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/htmltext/
---
## Shape.HtmlText property

Bu metin kutusunda veri ve bazı biçimleri içeren html dizesini alır ve ayarlar.

```csharp
public string HtmlText { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHtmlTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // HtmlText'in boş olup olmadığını kontrol edin ve gerekirse ayarlayın
            string html = shape.HtmlText;
            if (string.IsNullOrEmpty(html))
            {
                shape.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeHtmlTextDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


