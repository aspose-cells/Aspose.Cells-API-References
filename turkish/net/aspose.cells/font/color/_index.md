---
title: "Font.Color"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Fontun rengini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/font/color/
---
## Font.Color property

Yazı tipinin Rengini alır veya ayarlar.

```csharp
public Color Color { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Farklı yazı tipi renkleri ve stilleriyle HTML ayarla
            Cell cell = worksheet.Cells["A1"];
            cell.HtmlString = "<font color='Red'>Red Text</font> <font color='#0000FF'>Blue Text</font><font style='color:#00FF00;text-decoration: underline;'>Green Underlined</font>";
            
            // Zengin metin biçimlendirmesini al
            FontSetting[] richText = cell.GetCharacters();
            
            // Renk özelliklerini doğrula ve göster
            Console.WriteLine("First segment color: " + richText[0].Font.Color);
            Console.WriteLine("Second segment color: " + richText[1].Font.Color);
            Console.WriteLine("Third segment underline: " + richText[2].Font.Underline);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FontColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


