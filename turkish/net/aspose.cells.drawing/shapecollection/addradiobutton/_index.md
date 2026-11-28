---
title: "ShapeCollection.AddRadioButton"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir RadioButton ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addradiobutton/
---
## ShapeCollection.AddRadioButton method

Çalışma sayfasına bir RadioButton ekler.

```csharp
public RadioButton AddRadioButton(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | RadioButton'ın sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | RadioButton'ın sol sütunundan yatay kaydırmasını piksel biriminde temsil eder. |
| yükseklik | Int32 | RadioButton'ın yüksekliğini piksel biriminde temsil eder. |
| genişlik | Int32 | RadioButton'ın genişliğini piksel biriminde temsil eder. |

### Dönüş Değeri

Bir RadioButton nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRadioButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir radyo düğmesi ekle
            Aspose.Cells.Drawing.RadioButton radioButton = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 50);
            radioButton.Text = "Option 1";

            // Çalışma kitabını kaydedin
            workbook.Save("RadioButtonDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [RadioButton](../../radiobutton/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


