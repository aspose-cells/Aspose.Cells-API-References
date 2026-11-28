---
title: "ShapeCollection.AddGroupBox"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir GroupBox ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

Çalışma sayfasına bir GroupBox ekler.

```csharp
public GroupBox AddGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | GroupBox'ın sol satırından dikey kaydırmasını, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | GroupBox'ın sol sütunundan yatay kaydırmasını, piksel biriminde temsil eder. |
| yükseklik | Int32 | GroupBox'ın yüksekliğini, piksel biriminde temsil eder. |
| genişlik | Int32 | GroupBox'ın genişliğini, piksel biriminde temsil eder. |

### Dönüş Değeri

Bir GroupBox nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddGroupBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir grup kutusu ekle
            ShapeCollection shapes = worksheet.Shapes;
            Aspose.Cells.Drawing.GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);

            // Çalışma kitabını kaydedin
            workbook.Save("GroupBoxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [GroupBox](../../groupbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


