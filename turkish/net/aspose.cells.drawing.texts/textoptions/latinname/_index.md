---
title: "TextOptions.LatinName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextOptions özelliği. Latin adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textoptions/latinname/
---
## TextOptions.LatinName property

Latin adını alır ve ayarlar.

```csharp
public string LatinName { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyLatinNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Metin seçeneklerini göstermek için bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.Text = "Sample Text";

            // Şeklin ilk paragrafından TextOptions'ı alın
            TextOptions textOptions = shape.TextBody.TextParagraphs[0].TextOptions;

            // Mevcut LatinName değerini göster
            Console.WriteLine("Current LatinName value: " + textOptions.LatinName);

            // Yeni bir LatinName değeri ayarlayın
            textOptions.LatinName = "Times New Roman";

            // Yazı tipi render'ını karşılaştırmak için başka bir şekil oluşturun
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 3, 0, 100, 150);
            shape2.Text = "Comparison Text";
            shape2.TextBody.TextParagraphs[0].TextOptions.LatinName = "Arial";

            // Etkileri görmek için çalışma kitabını kaydedin
            workbook.Save("PropertyLatinNameDemo.xlsx");

            // Yeni LatinName değerini göster
            Console.WriteLine("New LatinName value: " + textOptions.LatinName);
        }
    }
}
```

### Ayrıca Bakınız

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


