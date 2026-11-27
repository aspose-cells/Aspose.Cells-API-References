---
title: "HtmlTableLoadOption.OriginalSheetIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlTableLoadOption-egenskap. Hämta eller ange det ursprungliga indexet för kalkylbladet i HTML"
type: docs
url: /sv/net/aspose.cells/htmltableloadoption/originalsheetindex/
---
## HtmlTableLoadOption.OriginalSheetIndex property

Hämta eller ange det ursprungliga indexet för kalkylbladet i HTML.

```csharp
public int OriginalSheetIndex { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyOriginalSheetIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                OriginalSheetIndex = 1,
                TargetSheetIndex = 0
            };

            loadOptions.TableLoadOptions.Add(tableLoadOption);
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


