---
title: "StyleFlag.RightBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Sağ kenar ayarları uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/rightborder/
---
## StyleFlag.RightBorder property

Sağ kenar ayarları uygulanacak.

```csharp
public bool RightBorder { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyRightBorderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kenarlıklı bir stil oluştur
            Style borderStyle = workbook.CreateStyle();
            borderStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            borderStyle.Borders[BorderType.RightBorder].Color = System.Drawing.Color.Red;

            // Stil bayrağı oluşturun ve sağ kenarı etkinleştirin
            StyleFlag borderFlag = new StyleFlag();
            borderFlag.RightBorder = true;

            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["B2"];
            cell.SetStyle(borderStyle, borderFlag);

            // Çalışma kitabını kaydedin
            workbook.Save("RightBorderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


