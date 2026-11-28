---
title: "TwoColorGradient.Color1"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TwoColorGradient özelliği. İlk gradient rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/twocolorgradient/color1/
---
## TwoColorGradient.Color1 property

İlk geçiş rengini alır ve ayarlar.

```csharp
public Color Color1 { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor1Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Gradient doldurmasıyla bir stil oluşturun
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            // İki renkli gradient'i başlatın
            style.SetTwoColorGradient(
                Color.Red,
                Color.Blue,
                GradientStyleType.Vertical,
                variant: 1);
            
            // Gradient'i hücre stiline uygula
            cell.SetStyle(style);
            
            // İlk rengi oku
            TwoColorGradient gradient = style.GetTwoColorGradientSetting();
            Console.WriteLine("Current Color1 value: " + gradient.Color1);
            
            // Gradient rengini değiştir ve yeniden uygula
            gradient.Color1 = Color.Lime;
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            
            // Güncellemeyi doğrula
            Console.WriteLine("Updated Color1 value: " + gradient.Color1);
            
            // Çıktı dosyasında görsel gösterim
            cell.PutValue("Color1 Gradient Demo");
            worksheet.AutoFitColumn(0);
            workbook.Save("TwoColorGradientPropertyColor1Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


