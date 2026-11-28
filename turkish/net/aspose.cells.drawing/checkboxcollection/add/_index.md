---
title: "CheckBoxCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBoxCollection yöntemi. Bir checkBox'ı koleksiyona ekler"
type: docs
url: /tr/net/aspose.cells.drawing/checkboxcollection/add/
---
## CheckBoxCollection.Add method

Koleksiyona bir checkBox ekler.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| yükseklik | Int32 | CheckBox yüksekliği, piksel biriminde. |
| genişlik | Int32 | CheckBox genişliği, piksel biriminde. |

### Dönüş Değeri

[`CheckBox`](../../checkbox/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Int32 parametreleri (upperLeftRow, upperLeftColumn, height, width) kullanarak checkbox ekle
            int index = worksheet.CheckBoxes.Add(10, 2, 20, 100);
            
            CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Value = true;
            checkBox.LinkedCell = "B11";
            
            workbook.Save("CheckBoxDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


