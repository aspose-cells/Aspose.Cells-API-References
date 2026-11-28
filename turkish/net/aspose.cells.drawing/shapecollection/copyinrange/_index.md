---
title: "ShapeCollection.CopyInRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Aralıktaki şekilleri hedef aralığa kopyalar."
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

Aralıktaki şekilleri hedef aralığa kopyala.

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Kaynak şekiller. |
| ca | CellArea | Kaynak aralık. |
| destRow | Int32 | Hedef aralığın hedef satır indeksi. |
| destColumn | Int32 | Hedef aralığın hedef sütunu. |
| isContained | Boolean | Yalnızca aralık içinde bulunan şekilleri kopyalayıp kopyalamayacağını belirler. Doğru ise, sadece aralıktaki şekilleri kopyalar. Aksi takdirde, MS Office gibi çalışır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // Bir dikdörtgen şekli ekle
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Kopyalanacak hücre alanını tanımlayın
            CellArea area2 = new CellArea();
            area2.StartColumn = 1;
            area2.StartRow = 1;
            area2.EndColumn = 5;
            area2.EndRow = 11;

            // Belirtilen aralıktaki şekilleri kopyala
            shapes.CopyInRange(shapes, area2, 12, 1, false);

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeCopyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


