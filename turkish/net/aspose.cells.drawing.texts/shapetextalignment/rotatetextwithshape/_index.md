---
title: "ShapeTextAlignment.RotateTextWithShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeTextAlignment özelliği. Metnin şekil ile döndürülüp döndürülmediğini gösterir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/
---
## ShapeTextAlignment.RotateTextWithShape property

Şekilde metin döndürülüp döndürülmediğini gösterir.

```csharp
public bool RotateTextWithShape { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotateTextWithShapeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir metin kutusu şekli ekleyin
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Metin hizalama özelliklerine erişin
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            
            // RotateTextWithShape özelliğini ayarlayın
            textAlignment.RotateTextWithShape = true;

            // Etkiyi göstermek için şekli döndür
            shape.RotationAngle = 45;

            // Çalışma kitabını kaydedin
            workbook.Save("RotateTextWithShapeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


