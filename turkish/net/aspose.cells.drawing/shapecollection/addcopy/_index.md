---
title: "ShapeCollection.AddCopy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir şekil ekler ve kopyalar"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addcopy/
---
## AddCopy(Shape, int, int, int, int) {#addcopy}

Çalışma sayfasına bir şekil ekler ve kopyalar.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceShape | Şekil | Kaynak şekil. |
| topRow | Int32 | Üst satır indeksi. |
| üst | Int32 | Şeklin üst satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol sütun indeksi. |
| sol | Int32 | Şeklin sol sütunundan yatay ofseti, piksel biriminde temsil eder. |

### Dönüş Değeri

Yeni [`Shape`](../../shape/) nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCopyWithShapeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // Bir dikdörtgen şekli ekle
            RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Yeni konumla dikdörtgen şeklinin bir kopyasını ekle
            shapes.AddCopy(rectangle, 7, 0, 7, 0);

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Shape, int, int, int, int, CopyOptions) {#addcopy_1}

Çalışma sayfasına bir şekil ekler ve kopyalar.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, 
    CopyOptions copyOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceShape | Şekil | Kaynak şekil. |
| topRow | Int32 | Üst satır indeksi. |
| üst | Int32 | Şeklin üst satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol sütun indeksi. |
| sol | Int32 | Şeklin sol sütunundan yatay ofseti, piksel biriminde temsil eder. |
| copyOptions | CopyOptions | Şekilleri kopyalama seçenekleri. |

### Dönüş Değeri

Yeni [`Shape`](../../shape/) nesnesi.

### Örnekler

```csharp

[C#]
//bir şekil ekle
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//Bir şekil ekler ve kopyalar.
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


