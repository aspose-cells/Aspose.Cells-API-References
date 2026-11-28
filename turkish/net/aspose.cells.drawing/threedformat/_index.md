---
title: "ThreeDFormat sınıfı."
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ThreeDFormat sınıfı. Bir şeklin üç boyutlu biçimlendirmesini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/
---
## ThreeDFormat class

Bir şeklin üç boyutlu biçimlendirmesini temsil eder.

```csharp
public class ThreeDFormat
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BottomBevelHeight](../../aspose.cells.drawing/threedformat/bottombevelheight/) { get; set; } | Alt köşegenin yüksekliğini alır ve ayarlar, ya da şekle ne kadar uygulandığını. Birim: Nokta. |
| [BottomBevelType](../../aspose.cells.drawing/threedformat/bottombeveltype/) { get; set; } | Alt köşegenin tipini alır ve ayarlar, ya da şekle ne kadar uygulandığını. Birim: Nokta. |
| [BottomBevelWidth](../../aspose.cells.drawing/threedformat/bottombevelwidth/) { get; set; } | Alt köşegenin genişliğini alır ve ayarlar, ya da şekle ne kadar uygulandığını. Birim: Nokta. |
| [ContourColor](../../aspose.cells.drawing/threedformat/contourcolor/) { get; set; } | Bir şeklin kontur rengini alır ve ayarlar. |
| [ContourWidth](../../aspose.cells.drawing/threedformat/contourwidth/) { get; set; } | Şeklin kontur genişliğini alır ve ayarlar, birim: nokta. |
| [ExtrusionColor](../../aspose.cells.drawing/threedformat/extrusioncolor/) { get; set; } | Bir şeklin ekstrüzyon rengini alır. |
| [ExtrusionHeight](../../aspose.cells.drawing/threedformat/extrusionheight/) { get; set; } | Şekle uygulanan ekstrüzyon yüksekliğini alır ve ayarlar, birim: nokta. |
| [LightAngle](../../aspose.cells.drawing/threedformat/lightangle/) { get; set; } | Ekstrüzyon ışıklarının açısını alır ve ayarlar. |
| [Lighting](../../aspose.cells.drawing/threedformat/lighting/) { get; set; } | Işık düzeninin tipini alır ve ayarlar. |
| [LightingDirection](../../aspose.cells.drawing/threedformat/lightingdirection/) { get; set; } | Işık düzeninin sahneyle ilişkili olarak yönlendirildiği yönü alır ve ayarlar. |
| [Material](../../aspose.cells.drawing/threedformat/material/) { get; set; } | Bir şeklin son görünüm ve hissini vermek için aydınlatma özellikleriyle birleştirilen ön ayarlı malzemeyi temsil eder. |
| [Perspective](../../aspose.cells.drawing/threedformat/perspective/) { get; set; } | Bir ThreeDFormat nesnesinin görüntülenebileceği açıyı alır ve ayarlar. |
| [PresetCameraType](../../aspose.cells.drawing/threedformat/presetcameratype/) { get; set; } | Ekstrüzyon ön ayarlı kamera tipini alır ve ayarlar. |
| [RotationX](../../aspose.cells.drawing/threedformat/rotationx/) { get; set; } | Ekstrüde şeklin x ekseni etrafındaki dönüşünü derece cinsinden alır ve ayarlar. |
| [RotationY](../../aspose.cells.drawing/threedformat/rotationy/) { get; set; } | Ekstrüde şeklin y ekseni etrafındaki dönüşünü derece cinsinden alır ve ayarlar. |
| [RotationZ](../../aspose.cells.drawing/threedformat/rotationz/) { get; set; } | Ekstrüde şeklin z ekseni etrafındaki dönüşünü derece cinsinden alır ve ayarlar. |
| [TopBevelHeight](../../aspose.cells.drawing/threedformat/topbevelheight/) { get; set; } | Üst köşegenin yüksekliğini alır ve ayarlar, ya da şekle ne kadar uygulandığını. Birim: Nokta. |
| [TopBevelType](../../aspose.cells.drawing/threedformat/topbeveltype/) { get; set; } | Üst köşebentinin tipini alır ve ayarlar, ya da şekle ne kadar uygulandığını. Birim olarak Puan. |
| [TopBevelWidth](../../aspose.cells.drawing/threedformat/topbevelwidth/) { get; set; } | Üst köşebentinin genişliğini alır ve ayarlar, ya da şekle ne kadar uygulandığını. Birim olarak Puan. |
| [Z](../../aspose.cells.drawing/threedformat/z/) { get; set; } | 3B şekil için yerden mesafeyi tanımlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/threedformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/threedformat/gethashcode/)() | Hash kodunu alır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassThreeDFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 210, 210, 200, 200);
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.ExtrusionHeight = 20;

            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


