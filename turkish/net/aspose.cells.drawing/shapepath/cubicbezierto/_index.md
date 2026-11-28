---
title: "ShapePath.CubicBezierTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePath yöntemi. Mevcut şekle bir kübik Bézier eğrisi ekler. Başlangıç noktası, mevcut şeklin bitiş noktasıdır. Birim Piksel"
type: docs
url: /tr/net/aspose.cells.drawing/shapepath/cubicbezierto/
---
## ShapePath.CubicBezierTo method

Mevcut şekle kübik Bézier eğrisi ekler. Başlangıç noktası, mevcut şeklin son noktasıdır. Unit: Pixel.

```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, 
    float endY)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ctrX1 | Single | Eğri için ilk kontrol noktasının x koordinatı (Birim: Piksel). |
| ctrY1 | Single | Eğri için ilk kontrol noktasının y koordinatı (Birim: Piksel). |
| ctrX2 | Single | Eğri için ikinci kontrol noktasının x koordinatı (Birim: Piksel). |
| ctrY2 | Single | Eğri için ikinci kontrol noktasının y koordinatı (Birim: Piksel). |
| endX | Single | Eğri son noktasının x koordinatı (Birim: Piksel). |
| endY | Single | Eğri son noktasının y koordinatı (Birim: Piksel). |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCubicBezierToWithSingleSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            //Yeni bir şekil yolu oluştur
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                        96.5f, -7.148871f,
                        130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                        182.24997f, 75.351f,
                        201, 120.517795f);
            shapePath1.MoveTo(150, 70);
            shapePath1.ArcTo(25, 25, 0, 270);


            //serbest form ekle
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath1 });

            // Sonucu kaydet
            workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


