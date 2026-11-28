---
title: "ShapeCollection.AddLabel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir Etiket ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

Çalışma sayfasına bir Label ekler.

```csharp
public Label AddLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Etiket'in sol satırından dikey kaymasını piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Etiket'in sol sütunundan yatay kaymasını piksel biriminde temsil eder. |
| yükseklik | Int32 | Etiket'in yüksekliğini piksel biriminde temsil eder. |
| genişlik | Int32 | Etiket'in genişliğini piksel biriminde temsil eder. |

### Dönüş Değeri

Bir Etiket nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLabelWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // Çalışma sayfasına bir etiket ekle
            Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
            label.Text = "Sample Label";

            // Çalışma kitabını kaydedin
            workbook.Save("AddLabelDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


