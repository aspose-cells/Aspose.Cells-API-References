---
title: "Shape.HeightInShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin, üst ebeveyn şeklinin üst kenarından, ebeveyn şeklin yüksekliğinin 1/4000 birimi cinsinden dikey offsetini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing/shape/heightinshape/
---
## Shape.HeightInShape property

Şeklin, üst ana şeklin üst kenarından dikey ofsetini, ana şeklin yüksekliğinin 1/4000 birimi olarak temsil eder.

```csharp
public int HeightInShape { get; set; }
```

### Açıklamalar

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInShapeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk olarak tüm gerekli parametrelerle şekilleri ekleyin
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 10, 10);
            Shape oval = worksheet.Shapes.AddOval(0, 0, 100, 100, 10, 120);

            // Şekilleri grupla
            Shape[] shapes = { rectangle, oval };
            GroupShape groupShape = worksheet.Shapes.Group(shapes);

            // Dikdörtgenin yüksekliğini üst grup şekline göre ayarla (üst yüksekliğin 1/4000'i)
            rectangle.HeightInShape = 2000; // Half the height of the parent
            oval.HeightInShape = 4000; // Full height of the parent

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeHeightInShapeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


