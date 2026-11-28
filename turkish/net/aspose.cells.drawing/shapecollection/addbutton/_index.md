---
title: "ShapeCollection.AddButton"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir Button ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addbutton/
---
## ShapeCollection.AddButton method

Çalışma sayfasına bir Düğme ekler.

```csharp
public Button AddButton(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Button'ın sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Button'ın sol sütunundan yatay ofseti, piksel biriminde temsil eder. |
| yükseklik | Int32 | Button'ın yüksekliğini, piksel biriminde temsil eder. |
| genişlik | Int32 | Button'ın genişliğini, piksel biriminde temsil eder. |

### Dönüş Değeri

Bir Button nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Belirtilen parametreleri kullanarak bir button ekle
            Aspose.Cells.Drawing.Button button = worksheet.Shapes.AddButton(1, 0, 1, 0, 100, 50);
            button.Text = "Click Me";

            // Çalışma kitabını kaydedin
            workbook.Save("ButtonDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Button](../../button/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


