---
title: "TextBoxCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxCollection yöntemi. Koleksiyona bir metin kutusu ekler"
type: docs
url: /tr/net/aspose.cells.drawing/textboxcollection/add/
---
## TextBoxCollection.Add method

Koleksiyona bir metin kutusu ekler.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| yükseklik | Int32 | Metin kutusunun yüksekliği, piksel biriminde. |
| genişlik | Int32 | Metin kutusunun genişliği, piksel biriminde. |

### Dönüş Değeri

[`TextBox`](../../textbox/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int index = worksheet.TextBoxes.Add(1, 1, 50, 100);
            Console.WriteLine("TextBox added at index: " + index);
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


