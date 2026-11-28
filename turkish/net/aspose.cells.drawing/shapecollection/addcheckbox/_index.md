---
title: "ShapeCollection.AddCheckBox"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir onay kutusu ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addcheckbox/
---
## ShapeCollection.AddCheckBox method

Çalışma sayfasına bir onay kutusu ekler.

```csharp
public CheckBox AddCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Onay kutusunun üst satırından dikey kaymasını piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Metin kutusunun sol sütunundan yatay offsetini piksel biriminde temsil eder. |
| yükseklik | Int32 | Metin kutusunun yüksekliği, piksel biriminde. |
| genişlik | Int32 | Metin kutusunun genişliği, piksel biriminde. |

### Dönüş Değeri

Yeni CheckBox nesnesinin indeksi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCheckBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // Belirtilen parametreleri kullanarak bir CheckBox ekle
            Aspose.Cells.Drawing.CheckBox checkBox = shapes.AddCheckBox(1, 0, 1, 0, 100, 50);

            // Çalışma kitabını kaydedin
            workbook.Save("CheckBoxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CheckBox](../../checkbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


