---
title: "GradientFill.SetTwoColorGradient"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GradientFill yöntemi. Belirtilen dolguyu iki renkli bir gradyana ayarlar. Yalnızca Excel 2007 için geçerlidir"
type: docs
url: /tr/net/aspose.cells.drawing/gradientfill/settwocolorgradient/
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetTwoColorGradientWithColorColorGradientStyleTyInt32Demo
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

                // SetTwoColorGradient'i gerçekçi parametrelerle çağır
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    Color.Blue,         // color2
                    GradientStyleType.DiagonalDown,  // style
                    1);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, Blue, DiagonalDown, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Etkiyi göstermek için çalışma kitabını kaydedin
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
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

    public class GradientFillMethodSetTwoColorGradientWithColorDoubleColorDoubleGradient297116Demo
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

                // SetTwoColorGradient'i gerçekçi parametrelerle çağır
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    0.5,                // transparency1 (50% transparent)
                    Color.Blue,         // color2
                    0.3,                // transparency2 (30% transparent)
                    GradientStyleType.Horizontal,  // style
                    2);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, 0.5, Blue, 0.3, Horizontal, 2)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Etkiyi göstermek için çalışma kitabını kaydedin
            workbook.Save("SetTwoColorGradientWithTransparencyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


