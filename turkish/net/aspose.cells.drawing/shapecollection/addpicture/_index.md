---
title: "ShapeCollection.AddPicture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Koleksiyona bir resim ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addpicture/
---
## AddPicture(int, int, int, int, Stream) {#addpicture}

Koleksiyona bir Picture ekler.

```csharp
public Picture AddPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| bottomRow | Int32 | Alt sağ satır indeksi |
| rightColumn | Int32 | Alt sağ sütun indeksi |
| akış | Stream | Görüntü verisini içeren akış nesnesi. |

### Dönüş Değeri

[`Picture`](../../picture/) Picture object.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddPictureWithInt32Int32Int32Int32StreamDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // Dosya akışından bir resim ekle
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                Picture picture = shapes.AddPicture(1, 0, 1, 0, fs);
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

---

## AddPicture(int, int, Stream, int, int) {#addpicture_1}

Koleksiyona bir Picture ekler.

```csharp
public Picture AddPicture(int topRow, int leftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| akış | Stream | Görüntü verisini içeren akış nesnesi. |
| widthScale | Int32 | Görüntü genişliğinin ölçeği, yüzde olarak. |
| heightScale | Int32 | Görüntü yüksekliğinin ölçeği, yüzde olarak. |

### Dönüş Değeri

[`Picture`](../../picture/) Picture object.

### Örnekler

```csharp

[C#]
//bir resim ekle
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    Picture picture = shapes.AddPicture(1, 1, fs, 50, 60);
}
```

### Ayrıca Bakınız

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


