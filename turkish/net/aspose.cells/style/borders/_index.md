---
title: "Style.Borders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Stilin BorderCollection'ını alır"
type: docs
url: /tr/net/aspose.cells/style/borders/
---
## Style.Borders property

Stilin [`BorderCollection`](../../bordercollection/) öğesini alır.

```csharp
public BorderCollection Borders { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBordersDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücreyi ve stilini al
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Farklı kenar stilleri ayarla
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            
            // Stili hücreye uygulayın
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("BorderStylesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


