---
title: "ShapeCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Şekli kaldır"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/removeat/
---
## ShapeCollection.RemoveAt method

Şekli kaldır.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Şeklin indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekiller koleksiyonunu al
            ShapeCollection shapes = worksheet.Shapes;

            // İlk dikdörtgen şekli ekle
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // İkinci dikdörtgen şekli ekle
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // İndeks 0'da bulunan ilk şekli kaldır
            shapes.RemoveAt(0);

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeCollectionRemoveAtDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


