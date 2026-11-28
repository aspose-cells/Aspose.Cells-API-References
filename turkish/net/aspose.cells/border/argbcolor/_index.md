---
title: "Border.ArgbColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Border özelliği. 32 bit ARGB değeriyle rengi alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/border/argbcolor/
---
## Border.ArgbColor property

32-bit ARGB değeriyle rengi alır ve ayarlar.

```csharp
public int ArgbColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // B2 hücresine eriş ve bir değer ayarla
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Border ARGB Color Demo");

            // Stili ve kenarlıkları al
            Style style = cell.GetStyle();
            Border border = style.Borders[BorderType.TopBorder];

            // ARGB rengi dahil kenarlık özelliklerini ayarla
            border.LineStyle = CellBorderType.Thick;
            unchecked
            {
                border.ArgbColor = (int)0xFFFF0000; // Red color in ARGB format with unchecked cast
            }

            // Değiştirilen stili hücreye uygula
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("BorderArgbColorDemo.xlsx");

            // ARGB renginin doğru ayarlandığını doğrula
            Border savedBorder = workbook.Worksheets[0].Cells["B2"].GetStyle().Borders[BorderType.TopBorder];
            Console.WriteLine("ARGB Color of top border: " + savedBorder.ArgbColor.ToString("X8"));
        }
    }
}
```

### Ayrıca Bakınız

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


