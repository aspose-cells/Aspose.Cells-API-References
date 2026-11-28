---
title: "PictureCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PictureCollection yöntemi. Koleksiyona bir resim ekler"
type: docs
url: /tr/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Koleksiyona bir Picture ekler.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| bottomRow | Int32 | Alt sağ satır indeksi |
| rightColumn | Int32 | Alt sağ sütun indeksi |
| akış | Stream | Görüntü verisini içeren akış nesnesi. |

### Dönüş Değeri

[`Picture`](../../picture/) object index.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32Int32Int32StreamDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Akıştan bir resim ekle
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(10, 10, 200, 200, fs);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Koleksiyona bir Picture ekler.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, string fileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| bottomRow | Int32 | Alt sağ satır indeksi |
| rightColumn | Int32 | Alt sağ sütun indeksi |
| fileName | String | Görüntü dosya adı. |

### Dönüş Değeri

[`Picture`](../../picture/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, 5, 5, "image.jpg");

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Koleksiyona bir Picture ekler.

```csharp
public int Add(int topRow, int leftColumn, Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| akış | Stream | Görüntü verisini içeren akış nesnesi. |

### Dönüş Değeri

[`Picture`](../../picture/) object index.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StreamDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Akıştan bir resim ekle
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(1, 1, fs);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Koleksiyona bir Picture ekler.

```csharp
public int Add(int topRow, int leftColumn, string fileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| fileName | String | Görüntü dosya adı. |

### Dönüş Değeri

[`Picture`](../../picture/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, "image.jpg");

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Koleksiyona bir Picture ekler.

```csharp
public int Add(int topRow, int leftColumn, Stream stream, int widthScale, int heightScale)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| akış | Stream | Görüntü verisini içeren akış nesnesi. |
| widthScale | Int32 | Görüntü genişliğinin ölçeği, yüzde olarak. |
| heightScale | Int32 | Görüntü yüksekliğinin ölçeği, yüzde olarak. |

### Dönüş Değeri

[`Picture`](../../picture/) object index.

### Örnekler

```csharp

[C#]
//bir resim ekle
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Ayrıca Bakınız

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Koleksiyona bir Picture ekler.

```csharp
public int Add(int topRow, int leftColumn, string fileName, int widthScale, int heightScale)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| fileName | String | Görüntü dosya adı. |
| widthScale | Int32 | Görüntü genişliğinin ölçeği, yüzde olarak. |
| heightScale | Int32 | Görüntü yüksekliğinin ölçeği, yüzde olarak. |

### Dönüş Değeri

[`Picture`](../../picture/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, "image.jpg", 50, 50);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


