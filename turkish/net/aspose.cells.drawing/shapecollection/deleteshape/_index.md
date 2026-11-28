---
title: "ShapeCollection.DeleteShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Bir şekli sil. Şekil grup içinde ise veya bir yorum şekli ise silinmez"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/deleteshape/
---
## ShapeCollection.DeleteShape method

Bir şekli sil. Şekil grup içinde ise veya bir yorum şekli ise silinmeyecek.

```csharp
public void DeleteShape(Shape shape)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| şekil | Şekil |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteShapeWithShapeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // İlk dikdörtgen şekli ekle
            Shape firstShape = shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // İkinci dikdörtgen şekli ekle
            Shape secondShape = shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // İlk şekli sil
            shapes.DeleteShape(firstShape);

            // Çalışma kitabını kaydedin
            workbook.Save("DeleteShapeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


