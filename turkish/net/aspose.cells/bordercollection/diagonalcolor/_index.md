---
title: "BorderCollection.DiagonalColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BorderCollection özelliği. Çapraz çizgilerin rengini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/bordercollection/diagonalcolor/
---
## BorderCollection.DiagonalColor property

Çapraz çizgilerin Rengini alır veya ayarlar.

```csharp
public Color DiagonalColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Border Demo");

            Style style = cell.GetStyle();
            
            // Çapraz kenarlık özelliklerini ayarlama
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Thick;

            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


