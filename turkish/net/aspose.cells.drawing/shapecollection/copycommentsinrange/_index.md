---
title: "ShapeCollection.CopyCommentsInRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Aralıktaki tüm yorumları kopyala"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/copycommentsinrange/
---
## ShapeCollection.CopyCommentsInRange method

Aralıktaki tüm yorumları kopyala.

```csharp
public void CopyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| şekiller | ShapeCollection | Kaynak şekiller. |
| ca | CellArea | Kaynak aralık. |
| destRow | Int32 | Hedef aralığın başlangıç satırı. |
| destColumn | Int32 | Hedef aralığın başlangıç sütunu. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyCommentsInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yorum ekle
            CommentCollection comments = worksheet.Comments;
            
            // A1 hücresine yorum ekle
            int commentIndex = comments.Add(0, 0);
            Comment comment = comments[commentIndex];
            comment.Note = "First note.";
            comment.Font.Name = "Times New Roman";
            
            // B2 hücresine yorum ekle
            comments.Add("B2");
            comment = comments["B2"];
            comment.Note = "Second note.";
            
            // Kaynak aralığı tanımla
            CellArea sourceArea = new CellArea();
            sourceArea.StartRow = 0;
            sourceArea.StartColumn = 0;
            sourceArea.EndRow = 1;
            sourceArea.EndColumn = 1;
            
            // Şekil koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;
            
            // Yorumları kaynak aralıktan hedefe kopyala (satır 5, sütun 1'den başlayarak)
            shapes.CopyCommentsInRange(shapes, sourceArea, 5, 1);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


