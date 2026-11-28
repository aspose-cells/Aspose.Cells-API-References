---
title: "Border.LineStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Border özelliği. Hücre kenarlık tipini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

Hücre kenarlık tipini alır veya ayarlar.

```csharp
public CellBorderType LineStyle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyLineStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücreye eriş ve stilini al
            Cell cell = worksheet.Cells["B2"];
            Style style = cell.GetStyle();

            // Farklı kenarlık çizgi stillerini ayarla
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;

            // Stili hücreye uygulayın
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("BorderLineStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


