---
title: "ShapeCollection.Remove"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Şekli kaldır"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

Şekli kaldır.

```csharp
public void Remove(Shape shape)
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
    public class ShapeCollectionMethodRemoveWithShapeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // İlk dikdörtgen şekli ekle
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // İkinci dikdörtgen şekli ekle
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // İsme veya indexe göre ilk şekli al
            Shape shapeToRemove = shapes["Rectangle 1"]; // or shapes[0];
            
            if (shapeToRemove != null)
            {
                // Şekli koleksiyondan kaldır
                shapes.Remove(shapeToRemove);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeRemoveDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


