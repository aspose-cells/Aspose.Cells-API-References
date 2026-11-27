---
title: "FileFontSource.FileFontSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFontSource konstruktor. Ctor"
type: docs
url: /sv/net/aspose.cells/filefontsource/filefontsource/
---
## FileFontSource constructor

Konstruktor.

```csharp
public FileFontSource(string filePath)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | sökväg till teckensnittsfil |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourceMethodCtorWithStringDemo
    {
        public static void Run()
        {
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");

            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont";
            cell.SetStyle(style);

            workbook.Save("FileFontSourceExample.xlsx");
        }
    }
}
```

### Se även

* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


