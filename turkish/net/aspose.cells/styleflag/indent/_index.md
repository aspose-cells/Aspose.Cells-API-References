---
title: "StyleFlag.Indent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Girinti seviyesi ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/indent/
---
## StyleFlag.Indent property

Girinti seviyesi ayarı uygulanacak.

```csharp
public bool Indent { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyIndentDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Girinti seviyeli bir stil oluşturun
            Style style = workbook.CreateStyle();
            style.IndentLevel = 2;
            style.HorizontalAlignment = TextAlignmentType.Left;

            // Girinti özelliği ayarlanmış stil bayrağı oluşturun
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Indent = true;

            // Verileri hücrelere uygulayın
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                }
            }

            // Stili girintili bir şekilde bir aralığa uygulayın
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 5, 5);
            range.ApplyStyle(style, styleFlag);

            // Stilin uygulandığını doğrulayın
            Cell cell = worksheet.Cells["A1"];
            Style appliedStyle = cell.GetStyle();
            Console.WriteLine($"Indent Level: {appliedStyle.IndentLevel}");
            Console.WriteLine($"Alignment: {appliedStyle.HorizontalAlignment}");

            // Çalışma kitabını kaydedin
            workbook.Save("IndentStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


