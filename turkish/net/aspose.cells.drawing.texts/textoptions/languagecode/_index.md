---
title: "TextOptions.LanguageCode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextOptions özelliği. Kullanıcı arayüzü dilini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textoptions/languagecode/
---
## TextOptions.LanguageCode property

Kullanıcı arayüzü dilini alır ve ayarlar.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir şekil ekle ve metnini ayarla
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample text with language settings";

            // Şeklin metin seçenekleri için dil kodunu ayarla
            shape.TextOptions.LanguageCode = CountryCode.Japan;

            // Dil kodunu doğrula ve çıktısını al
            Console.WriteLine("Shape Text Language Code: " + shape.TextOptions.LanguageCode);

            // Çalışma kitabını kaydedin
            workbook.Save("TextOptionsLanguageDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


