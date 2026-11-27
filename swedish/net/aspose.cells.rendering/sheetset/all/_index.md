---
title: "SheetSet.All"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetSet-egenskap. Hämtar en uppsättning med alla blad i arbetsboken i deras ursprungliga ordning"
type: docs
url: /sv/net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

Hämtar en uppsättning med alla blad i arbetsboken i deras ursprungliga ordning.

```csharp
public static SheetSet All { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyAllDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med två kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Ställ in exempeldata i båda bladen
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Spara alla blad till markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.SheetSet = SheetSet.All;
            
            workbook.Save("output.md", saveOptions);
            Console.WriteLine("All sheets saved to markdown successfully.");
        }
    }
}
```

### Se även

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


