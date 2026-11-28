---
title: "Style.HasBorders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Stil için kenarlıkların ayarlanıp ayarlanmadığını kontrol eder"
type: docs
url: /tr/net/aspose.cells/style/hasborders/
---
## Style.HasBorders property

Stil için kenarlıkların ayarlanıp ayarlanmadığını kontrol eder.

```csharp
public bool HasBorders { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHasBordersDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // A1 hücresine eriş ve kenarlıkları olup olmadığını kontrol et (varsayılan olarak false olmalı)
            Cell cellA1 = cells["A1"];
            Console.WriteLine("Cell A1 has borders: " + cellA1.GetStyle().HasBorders);

            // Kenarlıklı bir stil oluştur
            Style styleWithBorders = workbook.CreateStyle();
            styleWithBorders.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            styleWithBorders.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Stili B1 hücresine uygula
            Cell cellB1 = cells["B1"];
            cellB1.SetStyle(styleWithBorders);

            // B1 hücresinin kenarlıkları olup olmadığını kontrol et (şimdi true olmalı)
            Console.WriteLine("Cell B1 has borders: " + cellB1.GetStyle().HasBorders);

            // Çalışma kitabını kaydedin
            workbook.Save("HasBordersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


