---
title: "TextOptions.Kerning"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextOptions özelliği. Bu metin çalıştırması için karakter kerning'inin gerçekleşeceği minimum yazı tipi boyutunu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textoptions/kerning/
---
## TextOptions.Kerning property

Bu metin çalıştırması için karakter aralığının gerçekleşeceği minimum yazı tipi boyutunu belirtir.

```csharp
public double Kerning { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyKerningDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kerning'i göstermek için metinli bir şekil ekleyin
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Kerning Demonstration Text";

            // Şeklin TextOptions'ını alın
            TextOptions textOptions = shape.TextOptions;

            // Mevcut kerning değerini göster
            Console.WriteLine("Current Kerning value: " + textOptions.Kerning);

            // Kerning'i 12 puana ayarla (kerning'in gerçekleşmesi için minimum yazı tipi boyutu)
            textOptions.Kerning = 12;

            // Kerning etkisini gözlemlemek için daha büyük bir yazı tipi boyutu ayarla
            textOptions.Size = 24;

            // Etkiyi görmek için çalışma kitabını kaydet
            workbook.Save("PropertyKerningDemo.xlsx");

            // Karşılaştırma için farklı kerning'e sahip başka bir şekil oluştur
            var shape2 = worksheet.Shapes.AddTextBox(10, 0, 1, 0, 200, 100);
            shape2.Text = "Comparison Text Without Kerning";
            shape2.TextOptions.Size = 24;
            shape2.TextOptions.Kerning = 0; // No kerning

            // Her iki örnekle de tekrar kaydet
            workbook.Save("PropertyKerningDemoWithComparison.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


