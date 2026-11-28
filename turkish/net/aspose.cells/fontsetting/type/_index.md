---
title: "FontSetting.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSetting özelliği. Metin düğümünün tipini alır"
type: docs
url: /tr/net/aspose.cells/fontsetting/type/
---
## FontSetting.Type property

Metin düğümünün tipini alır.

```csharp
public virtual TextNodeType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;  // Added this using directive
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücreye metin ekleyin
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Hücrenin karakterleri için yazı tipi ayarlarını alın
            FontSetting fontSetting = new FontSetting(0, 6, workbook.Worksheets);

            // Mevcut Type değerini göster
            Console.WriteLine("Current Type value: " + fontSetting.Type);

            // Tipin metin işleme üzerindeki etkisini gösterin
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("The text is a standard text run.");
            }
            else if (fontSetting.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("The text is part of a paragraph.");
            }
            else if (fontSetting.Type == TextNodeType.Equation)
            {
                Console.WriteLine("The text represents an equation.");
            }

            // Tipe göre farklı biçimlendirme uygulayın
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                fontSetting.Font.Color = System.Drawing.Color.Red;
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);
            }

            // Sonucu kaydet
            workbook.Save("FontSettingTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


