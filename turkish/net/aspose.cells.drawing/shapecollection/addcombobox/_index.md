---
title: "ShapeCollection.AddComboBox"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir ComboBox ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addcombobox/
---
## ShapeCollection.AddComboBox method

Çalışma sayfasına bir ComboBox ekler.

```csharp
public ComboBox AddComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | ComboBox'ın sol satırından dikey kaydırmasını piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | ComboBox'ın sol sütunundan yatay kaydırmasını piksel biriminde temsil eder. |
| yükseklik | Int32 | ComboBox'ın yüksekliğini piksel biriminde temsil eder. |
| genişlik | Int32 | ComboBox'ın genişliğini piksel biriminde temsil eder. |

### Dönüş Değeri

Bir ComboBox nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddComboBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // Belirtilen parametrelerle bir combo box ekleyin
            Aspose.Cells.Drawing.ComboBox comboBox = shapes.AddComboBox(1, 0, 1, 0, 100, 50);

            // Hücre değerlerini ayarlayarak combo box'a öğeler ekleyin
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Combo kutusu için giriş aralığını ayarlayın
            comboBox.InputRange = "A1:A3";
            comboBox.DropDownLines = 3;

            // Çalışma kitabını kaydedin
            workbook.Save("AddComboBoxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ComboBox](../../combobox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


