---
title: "ShapeCollection.AddIcons"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. svg görüntüsü ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addicons/
---
## ShapeCollection.AddIcons method

svg görüntüsü ekler.

```csharp
public Picture AddIcons(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageByteData, byte[] compatibleImageData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Şeklin sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Şeklin sol sütunundan yatay ofseti, piksel biriminde. |
| yükseklik | Int32 | Şeklin yüksekliği, piksel biriminde. |
| genişlik | Int32 | Şeklin genişliği, piksel biriminde. |
| imageByteData | Byte[] | Görüntü bayt verisi. |
| compatibleImageData | Byte[] | Excel 2016 ve daha düşük sürümlerle uyumlu olması için svg'den dönüştürülmüş görüntü verisi. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddIconsWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Örnek bir simge dosyası oluşturun (gerçek kullanımda mevcut bir dosya kullanırsınız)
            string iconPath = "icon.svg";
            File.WriteAllText(iconPath, "<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><circle cx='50' cy='50' r='40' fill='red'/></svg>");

            // Çalışma sayfasına simge ekle
            using (FileStream fs = new FileStream(iconPath, FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                Picture picture = shapes.AddIcons(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            // Temizleme (isteğe bağlı)
            File.Delete(iconPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


