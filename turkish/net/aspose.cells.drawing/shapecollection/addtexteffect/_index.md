---
title: "ShapeCollection.AddTextEffect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Bir WordArt nesnesi ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addtexteffect/
---
## ShapeCollection.AddTextEffect method

Bir WordArt nesnesi ekler.

```csharp
public Shape AddTextEffect(MsoPresetTextEffect effect, string text, string fontName, int size, 
    bool fontBold, bool fontItalic, int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| efekt | MsoPresetTextEffect | mso ön ayarlı metin efekti türü. |
| metin | String | WordArt metni. |
| fontName | String | Yazı tipi adı. |
| boyut | Int32 | Yazı tipi boyutu |
| fontBold | Boolean | Yazı tipinin kalın olup olmadığını gösterir. |
| fontItalic | Boolean | Yazı tipinin italik olup olmadığını gösterir. |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Şeklin sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Şeklin sol sütunundan yatay kaydırmasını, piksel biriminde temsil eder. |
| yükseklik | Int32 | Şeklin yüksekliğini, piksel biriminde temsil eder. |
| genişlik | Int32 | Şeklin genişliğini, piksel biriminde temsil eder. |

### Dönüş Değeri

Yeni WordArt nesnesini temsil eden bir Shape nesnesi döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape wordArt = shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect10,
                "Sample WordArt",
                "Arial",
                18,
                false,
                false,
                3,
                0,
                3,
                0,
                200,
                50
            );

            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


