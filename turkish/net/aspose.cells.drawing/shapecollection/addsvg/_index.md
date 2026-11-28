---
title: "ShapeCollection.AddSvg"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. svg görüntüsü ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addsvg/
---
## ShapeCollection.AddSvg method

svg görüntüsü ekler.

```csharp
public Picture AddSvg(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] svgData, byte[] compatibleImageData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Şeklin sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Şeklin sol sütunundan yatay ofseti, piksel biriminde. |
| yükseklik | Int32 | Şeklin yüksekliği, piksel biriminde. |
| genişlik | Int32 | Şeklin genişliği, piksel biriminde. |
| svgData | Byte[] | svg görüntü verisi. |
| compatibleImageData | Byte[] | Excel 2016 ve daha düşük sürümlerle uyumlu olması için svg'den dönüştürülmüş görüntü verisi. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSvgWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.ShapeCollection shapes = worksheet.Shapes;

            // SVG dosyasını yükle
            using (FileStream fs = new FileStream("image.svg", FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                
                // SVG'yi çalışma sayfasına ekle
                Aspose.Cells.Drawing.Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


