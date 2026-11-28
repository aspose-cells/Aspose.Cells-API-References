---
title: "TwoColorGradient.Color2"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TwoColorGradient özelliği. İkinci gradient rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/twocolorgradient/color2/
---
## TwoColorGradient.Color2 property

İkinci geçiş rengini alır ve ayarlar.

```csharp
public Color Color2 { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor2Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İki renkli bir gradient örneği oluşturun
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.Green,
                GradientStyleType.Horizontal,
                1);

            // İlk stili başlangıç gradient'iyle oluşturun
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].PutValue("Initial Gradient");
            worksheet.Cells["A1"].SetStyle(style1);

            // Mevcut Color2 değerini gösterin
            System.Console.WriteLine("Current Color2: " + gradient.Color2);

            // Color2 özelliğini değiştirin
            gradient.Color2 = Color.Red;

            // Değiştirilmiş gradient ile ikinci stili oluşturun
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A2"].PutValue("Modified Gradient");
            worksheet.Cells["A2"].SetStyle(style2);

            // Görünürlük için satırları ayarlayın
            worksheet.Cells.SetRowHeight(0, 40);
            worksheet.Cells.SetRowHeight(1, 40);

            // Çalışma kitabını kaydedin
            workbook.Save("TwoColorGradientColor2Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


