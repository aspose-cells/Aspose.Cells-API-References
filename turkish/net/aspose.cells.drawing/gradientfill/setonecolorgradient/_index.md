---
title: "GradientFill.SetOneColorGradient"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GradientFill yöntemi. Belirtilen dolguyu tek renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir"
type: docs
url: /tr/net/aspose.cells.drawing/gradientfill/setonecolorgradient/
---
## GradientFill.SetOneColorGradient method

Belirtilen dolguyu tek renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | Color | Bir degrade rengi. |
| derece | Double | Degrade derecesi. 0.0 (koyu) ile 1.0 (açık) arasında bir değer olabilir. |
| stil | GradientStyleType | Degrade gölgelendirme stili. |
| variant | Int32 | Degrade varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Degrade sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Degrade dolgu uygulamak için bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Dolgu tipini degrade olarak ayarla
                shape.Fill.FillType = FillType.Gradient;

                // Degrade dolguyu al
                GradientFill gradientFill = shape.Fill.GradientFill;
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Gerçekçi parametrelerle SetOneColorGradient'i çağır
                gradientFill.SetOneColorGradient(
                    Color.Green,        // color
                    0.7,                // degree (70% intensity)
                    GradientStyleType.DiagonalUp,  // style
                    1);                 // variant

                Console.WriteLine("SetOneColorGradient method called successfully with parameters (Green, 0.7, DiagonalUp, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }

            // Etkiyi göstermek için çalışma kitabını kaydedin
            workbook.Save("SetOneColorGradientDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


