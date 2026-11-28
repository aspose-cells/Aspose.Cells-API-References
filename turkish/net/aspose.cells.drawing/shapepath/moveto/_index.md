---
title: "ShapePath.MoveTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePath yöntemi. Mevcut şekli kapatmadan belirtilen noktadan yeni bir şekil başlatır. Yola eklenen sonraki tüm noktalar bu yeni şekle eklenir. Birim: Piksel"
type: docs
url: /tr/net/aspose.cells.drawing/shapepath/moveto/
---
## ShapePath.MoveTo method

Belirtilen noktadan mevcut şekli kapatmadan yeni bir şekil başlatır. Yola eklenen sonraki tüm noktalar bu yeni şekle eklenir. Unit: Pixel.

```csharp
public void MoveTo(float x, float y)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| x | Single | Şeklin başlangıç noktasının x koordinatı (Birim: Piksel). |
| y | Single | Şeklin başlangıç noktasının y koordinatı (Birim: Piksel). |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodMoveToWithSingleSingleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Yeni bir şekil yolu oluştur
                ShapePath shapePath = new ShapePath();

                // Başlangıç noktasına git
                shapePath.MoveTo(10, 10);

                // (Single, Single) parametreleriyle LineTo yöntemini çağır
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                //serbest form ekle
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
           
            
            // Sonucu kaydet
            workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


