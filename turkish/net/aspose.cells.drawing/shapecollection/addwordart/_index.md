---
title: "ShapeCollection.AddWordArt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Excel 2007'den beri önceden ayarlanmış WordArt ekler."
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addwordart/
---
## ShapeCollection.AddWordArt method

Excel 2007'den beri önceden ayarlanmış WordArt ekler.

```csharp
public Shape AddWordArt(PresetWordArtStyle style, string text, int topRow, int top, int leftColumn, 
    int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | PresetWordArtStyle | Önceden ayarlanmış WordArt stili. |
| metin | String | Metin. |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Şeklin sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Şeklin sol sütunundan yatay kaydırmasını, piksel biriminde temsil eder. |
| yükseklik | Int32 | Şeklin yüksekliğini, piksel biriminde temsil eder. |
| genişlik | Int32 | Şeklin genişliğini, piksel biriminde temsil eder. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddWordArtWithPresetWordArtStyleStringInt32IDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // Belirtilen parametrelerle bir WordArt ekle
            Shape wordArt = shapes.AddWordArt(
                PresetWordArtStyle.WordArtStyle1, 
                "Sample WordArt", 
                10,  // left
                10,  // top
                200, // width
                50,  // height
                100, // rotation
                200  // z-order
            );

            // Çalışma kitabını kaydedin
            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [PresetWordArtStyle](../../presetwordartstyle/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


