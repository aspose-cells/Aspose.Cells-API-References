---
title: "ShapeCollection.AddFreeFloatingShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına serbest yüzen bir şekil ekler. Yalnızca çizgi/görüntü şekli için geçerlidir"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addfreefloatingshape/
---
## ShapeCollection.AddFreeFloatingShape method

Çalışma sayfasına serbest yüzen bir şekil ekler. Yalnızca çizgi/görsel şekil için geçerlidir.

```csharp
public Shape AddFreeFloatingShape(MsoDrawingType type, int top, int left, int height, int width, 
    byte[] imageData, bool isOriginalSize)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | MsoDrawingType | Şekil türü. |
| üst | Int32 | Şeklin çalışma sayfasının üst satırından dikey kaymasını piksel biriminde temsil eder. |
| sol | Int32 | Şeklin çalışma sayfasının sol sütunundan yatay kaymasını piksel biriminde temsil eder. |
| yükseklik | Int32 | LineShape'in yüksekliğini, piksel biriminde temsil eder. |
| genişlik | Int32 | LineShape'in genişliğini, piksel biriminde temsil eder. |
| imageData | Byte[] | Görüntü verisi, yalnızca resim için geçerlidir. |
| isOriginalSize | Boolean | Şekil bir resim ise orijinal boyutu kullanıp kullanmayacağını belirtir. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeFloatingShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Bir çizgi şekli ekleyin
            Shape floatingShape_Line = shapes.AddFreeFloatingShape(
                MsoDrawingType.Line, 
                100, 100, 100, 50, 
                null, 
                false);

            // Bir resim şekli ekleyin (örnek görüntü verisi kullanarak)
            byte[] imageData = null;
            try
            {
                using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
                {
                    imageData = new byte[fs.Length];
                    fs.Read(imageData, 0, (int)fs.Length);
                }
            }
            catch
            {
                // Dosya bulunamazsa sahte görüntü verisi oluşturun
                imageData = new byte[100];
            }

            Shape floatingShape_Picture = shapes.AddFreeFloatingShape(
                MsoDrawingType.Picture, 
                200, 100, 100, 50, 
                imageData, 
                false);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


