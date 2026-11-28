---
title: "ThreeDFormat.Material"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Bir şeklin son görünüm ve hissini sağlamak için aydınlatma özellikleriyle birleştirilen önceden ayarlanmış malzemeyi temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/material/
---
## ThreeDFormat.Material property

Bir şeklin son görünüm ve hissini vermek için aydınlatma özellikleriyle birleştirilen ön ayarlı malzemeyi temsil eder.

```csharp
public PresetMaterialType Material { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyMaterialDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 3D biçimlendirmeyi göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);
            shape.Text = "3D Material Demo";
            
            // Şeklin ThreeDFormat'ına eriş
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mevcut malzeme değerini göster
            Console.WriteLine("Current Material value: " + threeDFormat.Material);

            // Farklı malzeme tiplerini ayarlayın ve etkilerini gözlemleyin
            threeDFormat.Material = PresetMaterialType.Metal;
            Console.WriteLine("Material changed to Metal");

            threeDFormat.Material = PresetMaterialType.Plastic;
            Console.WriteLine("Material changed to Plastic");

            threeDFormat.Material = PresetMaterialType.Matte;
            Console.WriteLine("Material changed to Matte");

            // Malzeme etkisini daha iyi görmek için diğer 3D özelliklerini yapılandırın
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Çalışma kitabını 3D efektlerle kaydet
            workbook.Save("ThreeDFormatMaterialDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


