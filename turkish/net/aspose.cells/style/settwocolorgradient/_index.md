---
title: "Style.SetTwoColorGradient"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style yöntemi. Belirtilen doldurmayı iki renkli bir degradeye ayarlar"
type: docs
url: /tr/net/aspose.cells/style/settwocolorgradient/
---
## Style.SetTwoColorGradient method

Belirtilen doldurmayı iki renkli degradeye ayarlar.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color1 | Color | Bir degrade rengi. |
| color2 | Color | İki degrade rengi. |
| gradientStyleType | GradientStyleType | Degrade gölgelendirme stili. |
| variant | Int32 | Degrade varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Degrade sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir stil nesnesi oluşturun
            Style style = workbook.CreateStyle();

            // Stil için iki renkli degrade ayarla
            style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);

            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Gradient Style Demo");

            // Degrade ayarlarını doğrula
            Color color1, color2;
            GradientStyleType gradientStyle;
            int variant;
            style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);

            Console.WriteLine("Color1: " + color1);
            Console.WriteLine("Color2: " + color2);
            Console.WriteLine("Gradient Style: " + gradientStyle);
            Console.WriteLine("Variant: " + variant);

            // Çalışma kitabını kaydedin
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


