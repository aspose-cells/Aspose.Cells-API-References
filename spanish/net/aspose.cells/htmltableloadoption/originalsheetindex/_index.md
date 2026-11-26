---
title: "HtmlTableLoadOption.OriginalSheetIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlTableLoadOption. Obtenga o establezca el índice original de la hoja de cálculo en el HTML"
type: docs
url: /es/net/aspose.cells/htmltableloadoption/originalsheetindex/
---
## HtmlTableLoadOption.OriginalSheetIndex property

Obtener o establecer el índice original de la hoja de cálculo en el html.

```csharp
public int OriginalSheetIndex { get; set; }
```

### Ejemplos

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

### Ver también

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


