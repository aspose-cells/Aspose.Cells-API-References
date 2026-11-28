---
title: "StyleFlag.All"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Tüm özellikler uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

Tüm özellikler uygulanacak.

```csharp
public bool All { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyAllDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Katı kırmızı arka planlı bir stil oluşturun
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;

            // All özelliği true olarak ayarlanmış bir stil bayrağı oluşturun
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.All = true;

            // Stili ilk sütuna uygulayın
            Column column = cells.Columns[0];
            column.ApplyStyle(style, styleFlag);

            // Stilin sütundaki hücrelere uygulandığını doğrulayın
            Cell cell = cells[0, 0];
            Style appliedStyle = cell.GetStyle();
            
            Console.WriteLine("Pattern: " + appliedStyle.Pattern);
            Console.WriteLine("Color: " + appliedStyle.ForegroundColor);
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


