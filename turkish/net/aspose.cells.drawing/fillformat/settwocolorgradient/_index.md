---
title: "FillFormat.SetTwoColorGradient"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat yöntemi. Belirtilen doldurmayı iki renkli gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir."
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/settwocolorgradient/
---
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}

Belirtilen dolguyu iki renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color1 | Color | Bir degrade rengi. |
| color2 | Color | İki degrade rengi. |
| stil | GradientStyleType | Degrade gölgelendirme stili. |
| variant | Int32 | Degrade varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Degrade sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gradient doldurmayı göstermek için basit bir şekil oluştur
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 100, 100);

            // Şeklin doldurma formatını al
            FillFormat fillFormat = shape.Fill;

            // Belirtilen parametrelerle iki renkli gradient ayarla
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);

            // Çalışma kitabını kaydedin
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}

Belirtilen dolguyu iki renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir.

```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2, 
    double transparency2, GradientStyleType style, int variant)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color1 | Color | Bir degrade rengi. |
| transparency1 | Double | Renk1'in şeffaflık derecesi, 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak. |
| color2 | Color | İki degrade rengi. |
| transparency2 | Double | Renk2'nin şeffaflık derecesi, 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak. |
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

    public class FillFormatMethodSetTwoColorGradientWithColorDoubleColorDoubleGradientDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doldurma biçimlendirmesini göstermek için dikdörtgen şekil oluştur
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 150, 100);
            FillFormat fillFormat = rectangle.Fill;

            try
            {
                // SetTwoColorGradient için parametreleri hazırla
                Color color1 = Color.Red;
                double transparency1 = 0.3;
                Color color2 = Color.Blue;
                double transparency2 = 0.7;
                GradientStyleType gradientStyle = GradientStyleType.Horizontal;
                int variant = 1;

                // SetTwoColorGradient'ı belirli parametrelerle çağır
                fillFormat.SetTwoColorGradient(
                    color1, 
                    transparency1, 
                    color2, 
                    transparency2, 
                    gradientStyle, 
                    variant
                );

                Console.WriteLine("SetTwoColorGradient executed successfully with parameters (Color, Double, Color, Double, GradientStyleType, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTwoColorGradient: {ex.Message}");
            }

            // Etkisini göstermek için çalışma kitabını kaydedin
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


