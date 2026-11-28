---
title: "Shape.MoveToRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Şekli belirtilen bir aralığa taşır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/movetorange/
---
## Shape.MoveToRange method

Şekli belirtilen aralığa taşır.

```csharp
public void MoveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| bottomRow | Int32 | Alt sağ satır indeksi |
| rightColumn | Int32 | Alt sağ sütun indeksi |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodMoveToRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Şekli belirli bir aralığa taşıyın
            shape.MoveToRange(12, 3, 13, 5);

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeMoveToRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


