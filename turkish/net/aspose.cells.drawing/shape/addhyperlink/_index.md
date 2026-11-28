---
title: "Shape.AddHyperlink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Şekle bir hiperlink ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shape/addhyperlink/
---
## Shape.AddHyperlink method

Şekle bir köprü ekler.

```csharp
public Hyperlink AddHyperlink(string address)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| address | String | Köprünün adresi. |

### Dönüş Değeri

Yeni hiperlink nesnesini döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAddHyperlinkWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Şekle dize URL kullanarak bir hiperlink ekle
            Aspose.Cells.Hyperlink hyperlink = shape.AddHyperlink("https://www.aspose.com/");

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeWithHyperlink.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


