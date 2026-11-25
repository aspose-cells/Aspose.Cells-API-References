---
title: "HtmlTableLoadOption.OriginalSheetIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlTableLoadOption. Ottieni o imposta l'indice originale del foglio di lavoro nell'html"
type: docs
url: /it/net/aspose.cells/htmltableloadoption/originalsheetindex/
---
## HtmlTableLoadOption.OriginalSheetIndex property

Ottieni o imposta l'indice originale del foglio di lavoro nell'html.

```csharp
public int OriginalSheetIndex { get; set; }
```

### Esempi

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

### Vedi anche

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


