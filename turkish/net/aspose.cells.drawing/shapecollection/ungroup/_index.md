---
title: "ShapeCollection.Ungroup"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Şekil öğelerinin gruplamasını kaldırır"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/ungroup/
---
## ShapeCollection.Ungroup method

Şekil öğelerinin gruplarını çöz.

```csharp
public void Ungroup(GroupShape group)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| grup | GroupShape | Grup şekli. |

### Açıklamalar

Grup şekli başka bir grup şekli tarafından gruplanmışsa, hiçbir şey yapılmaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUngroupWithGroupShapeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // İlk dikdörtgen şekli ekle
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // İkinci dikdörtgen şekli ekle
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Gruplamak için şekillerin dizisini oluştur
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Şekilleri grupla
            GroupShape groupShape = shapes.Group(shapesArr);

            // Grup şeklinin gruplamasını kaldır
            shapes.Ungroup(groupShape);
        }
    }
}
```

### Ayrıca Bakınız

* class [GroupShape](../../groupshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


