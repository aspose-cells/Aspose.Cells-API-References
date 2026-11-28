---
title: "ShapeCollection.AddTextBox"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir metin kutusu ekler."
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

Çalışma sayfasına bir metin kutusu ekler.

```csharp
public TextBox AddTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Metin kutusunun üst satırından dikey offsetini piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Metin kutusunun sol sütunundan yatay offsetini piksel biriminde temsil eder. |
| yükseklik | Int32 | Metin kutusunun yüksekliğini piksel biriminde temsil eder. |
| genişlik | Int32 | Metin kutusunun genişliğini piksel biriminde temsil eder. |

### Dönüş Değeri

Bir [`TextBox`](../../textbox/) nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // Belirtilen konum ve boyutta bir TextBox ekle
            TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
            textBox.Text = "Sample TextBox";

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


