---
title: "Shape.AlignTopRightCorner"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape method. Resmi sağ üst köşeye taşır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/aligntoprightcorner/
---
## Shape.AlignTopRightCorner method

Resmi sağ üst köşeye taşır.

```csharp
public void AlignTopRightCorner(int topRow, int rightColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | satır indeksi. |
| rightColumn | Int32 | sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAlignTopRightCornerWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hizalamak için bir örnek şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Şeklin sağ üst köşesini satır 2, sütun 5'e hizala
            shape.AlignTopRightCorner(2, 5);

            // Çalışma kitabını kaydedin
            workbook.Save("AlignTopRightCornerDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


