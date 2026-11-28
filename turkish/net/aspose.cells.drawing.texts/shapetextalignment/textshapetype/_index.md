---
title: "ShapeTextAlignment.TextShapeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeTextAlignment özelliği. Metnin dönüşüm tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/textshapetype/
---
## ShapeTextAlignment.TextShapeType property

Metnin dönüşüm türünü alır ve ayarlar.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir metin kutusu şekli ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);

            // Şeklin metin hizalamasını al
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // TextShapeType özelliğini ayarlayın
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;

            // Çalışma kitabını kaydedin
            workbook.Save("TextShapeTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [AutoShapeType](../../../aspose.cells.drawing/autoshapetype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


