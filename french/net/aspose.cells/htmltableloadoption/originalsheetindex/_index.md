---
title: "HtmlTableLoadOption.OriginalSheetIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "HtmlTableLoadOption property. Obtenir ou définir l'indice original de la feuille de calcul dans le HTML"
type: docs
url: /fr/net/aspose.cells/htmltableloadoption/originalsheetindex/
---
## HtmlTableLoadOption.OriginalSheetIndex property

Obtenez ou définissez l'index original de la feuille de calcul dans le html.

```csharp
public int OriginalSheetIndex { get; set; }
```

### Exemples

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

### Voir aussi

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


