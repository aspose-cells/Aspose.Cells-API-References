---
title: "IndividualFontConfigs.IndividualFontConfigs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IndividualFontConfigs-konstruktor. Ctor"
type: docs
url: /sv/net/aspose.cells/individualfontconfigs/individualfontconfigs/
---
## IndividualFontConfigs constructor

Konstruktor.

```csharp
public IndividualFontConfigs()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IndividualFontConfigsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa laddningsalternativ med IndividualFontConfigs
            var loadOptions = new OdsLoadOptions
            {
                FontConfigs = new IndividualFontConfigs(),
                StandardFont = "Arial",
                StandardFontSize = 12
            };

            // Skapa en ny arbetsbok med standardarbetsblad
            var workbook = new Workbook(FileFormatType.Xlsx);
            
            // Få åtkomst till ett arbetsblad och lägg till lite text
            var worksheet = workbook.Worksheets[0];
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text with custom font configs");

            // Spara arbetsboken (laddningsalternativ behövs inte för sparning)
            workbook.Save("FontConfigsDemo.ods", SaveFormat.Ods);
        }
    }
}
```

### Se även

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


