---
title: "Shape.SetLinkedCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Kontrolün değerine bağlı aralığı ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/setlinkedcell/
---
## Shape.SetLinkedCell method

Denetimin değerine bağlı aralığı ayarlar.

```csharp
public void SetLinkedCell(string formula, bool isR1C1, bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Kontrolün değerine bağlı aralık. |
| isR1C1 | Boolean | Formülün R1C1 olarak biçimlendirilmesi gerekip gerekmediği. |
| isLocal | Boolean | Formülün yerel ayarlara göre biçimlendirilmesi gerekip gerekmediği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLinkedCellWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir kaydırma çubuğu şekli ekleyin
            Aspose.Cells.Drawing.Shape scrollBar = worksheet.Shapes.AddScrollBar(2, 0, 2, 0, 130, 30);

            // Kaydırma çubuğu değerini A12 hücresine bağlayın
            scrollBar.SetLinkedCell("$A$12", false, true);

            // Çalışma kitabını kaydedin
            workbook.Save("SetLinkedCellDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


