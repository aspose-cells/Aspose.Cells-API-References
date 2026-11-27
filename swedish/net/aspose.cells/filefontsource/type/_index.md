---
title: "FileFontSource.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFontSource egenskap. Returnerar typen av teckensnittskälla"
type: docs
url: /sv/net/aspose.cells/filefontsource/type/
---
## FileFontSource.Type property

Returnerar typen av teckensnittskälla.

```csharp
public override FontSourceType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            string fontFilePath = "CustomFont.ttf";
            
            // Skapa en FileFontSource‑instans
            FileFontSource fontSource = new FileFontSource(fontFilePath);
            
            // Demonstrera användning av Type-egenskapen
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            
            // Skapa arbetsbok och tillämpa teckensnitt
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Text with custom font");
            
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont";
            cell.SetStyle(style);
            
            workbook.Save("FontSourceDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FontSourceType](../../fontsourcetype/)
* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


