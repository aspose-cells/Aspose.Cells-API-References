---
title: "ShapePath.LineTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePath yöntemi. Mevcut şekle bir çizgi segmenti ekler. Başlangıç noktası, mevcut şeklin bitiş noktasıdır. Birim Piksel"
type: docs
url: /tr/net/aspose.cells.drawing/shapepath/lineto/
---
## ShapePath.LineTo method

Mevcut şekle bir çizgi segmenti ekler. Başlangıç noktası, mevcut şeklin son noktasıdır. Unit: Pixel.

```csharp
public void LineTo(float x, float y)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| x | Single | Çizgi segmentinin bitiş noktasının x koordinatı (Birim: Piksel). |
| y | Single | Çizgi segmentinin bitiş noktasının y koordinatı (Birim: Piksel). |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodLineToWithSingleSingleDemo
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

                Console.WriteLine("LineTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("ShapePathMethodLineToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


