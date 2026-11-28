---
title: "ThreeDFormat.PresetCameraType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Ekstrüzyon ön ayarlı kamera tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/presetcameratype/
---
## ThreeDFormat.PresetCameraType property

Ekstrüzyon ön ayarlı kamera tipini alır ve ayarlar.

```csharp
public PresetCameraType PresetCameraType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPresetCameraTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 3D biçimlendirmeyi göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 200);
            
            // Şeklin ThreeDFormat'ını al
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mevcut PresetCameraType değerini göster
            Console.WriteLine("Current PresetCameraType: " + threeDFormat.PresetCameraType);

            // Yeni bir PresetCameraType değeri ayarla
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveHeroicLeftFacing;

            // Etkiyi görünür kılmak için ek 3D biçimlendirme uygula
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Yeni PresetCameraType değerini göster
            Console.WriteLine("New PresetCameraType: " + threeDFormat.PresetCameraType);

            // Etkisini göstermek için çalışma kitabını kaydedin
            workbook.Save("ThreeDFormatPresetCameraTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PresetCameraType](../../presetcameratype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


