---
title: "ShapeCollection.DeleteInRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Aralıktaki şekilleri sil. Yorum şekilleri silinmeyecek"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

Aralıktaki şekilleri sil. Yorum şekilleri silinmeyecek.

```csharp
public void DeleteInRange(CellArea ca)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | CellArea | Aralık. Şekiller aralık içinde bulunuyorsa, kaldırılacak. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteInRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // İlk dikdörtgen şekli ekle
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // İkinci dikdörtgen şekli ekle
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Şekillerin silinmesi gereken aralığı tanımla
            CellArea area = new CellArea();
            area.StartColumn = 0;
            area.StartRow = 5;
            area.EndColumn = 5;
            area.EndRow = 8;

            // Belirtilen aralıktaki şekilleri sil
            shapes.DeleteInRange(area);

            // Çalışma kitabını kaydedin (isteğe bağlı)
            workbook.Save("ShapeDeleteInRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


