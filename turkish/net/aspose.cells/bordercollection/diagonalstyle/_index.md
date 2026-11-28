---
title: "BorderCollection.DiagonalStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BorderCollection özelliği. Çapraz çizgilerin stilini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/bordercollection/diagonalstyle/
---
## BorderCollection.DiagonalStyle property

Çapraz çizgilerin stilini alır veya ayarlar.

```csharp
public CellBorderType DiagonalStyle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir hücreyi ve stilini al
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Çapraz kenarlık özelliklerini ayarla
            style.Borders.DiagonalStyle = CellBorderType.Thin;
            style.Borders.DiagonalColor = Color.Red;
            
            // Stili hücreye uygulayın
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


