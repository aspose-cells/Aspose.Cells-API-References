---
title: "TwoColorGradient.Variant"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TwoColorGradient özelliği. Degrade varyantını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/twocolorgradient/variant/
---
## TwoColorGradient.Variant property

Geçiş varyantını alır ve ayarlar.

```csharp
public int Variant { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk varyantla iki renkli degrade oluştur
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.DarkBlue,
                GradientStyleType.Horizontal,
                1
            );

            // Stili oluştur ve A1 hücresine uygula
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Variant 1");

            // Mevcut varyant değerini göster
            System.Console.WriteLine("Current Variant value: " + gradient.Variant);

            // Varyant değerini değiştir
            gradient.Variant = 2;

            // Değiştirilmiş stili oluştur ve B1 hücresine uygula
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Variant 2");

            // Degraderi görselleştirmek için hücreleri daha uzun yap
            worksheet.Cells.Rows[0].Height = 150;

            workbook.Save("TwoColorGradientVariantDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


