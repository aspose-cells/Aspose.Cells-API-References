---
title: "StyleFlag.LeftBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Sol kenar ayarları uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/leftborder/
---
## StyleFlag.LeftBorder property

Sol kenar ayarları uygulanacak.

```csharp
public bool LeftBorder { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLeftBorderDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];

            // Bir aralık oluşturun ve sol kenar stilini uygulayın
            var range = worksheet.Cells.CreateRange(1, 1, 1, 1);
            range.PutValue("Left Border Demo", false, false);

            // Stil ve bayrak oluşturun
            var style = workbook.CreateStyle();
            var flag = new StyleFlag();

            // Sol kenar özelliklerini ayarlayın
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;
            flag.LeftBorder = true;

            // Stili sol kenar bayrağıyla uygulayın
            range.ApplyStyle(style, flag);

            // Sol kenarın uygulandığını doğrulayın
            var appliedStyle = worksheet.Cells[1, 1].GetStyle();
            Console.WriteLine($"Left border color: {appliedStyle.Borders[BorderType.LeftBorder].Color}");
            Console.WriteLine($"Left border style: {appliedStyle.Borders[BorderType.LeftBorder].LineStyle}");

            // Çalışma kitabını kaydedin
            workbook.Save("LeftBorderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


