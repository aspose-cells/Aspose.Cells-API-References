---
title: "HtmlTableLoadOptionCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlTableLoadOptionCollection-egenskap. Hämtar HtmlTableLoadOption-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/htmltableloadoptioncollection/item/
---
## HtmlTableLoadOptionCollection indexer

Hämtar [`HtmlTableLoadOption`](../../htmltableloadoption/) elementet på det angivna indexet.

```csharp
public HtmlTableLoadOption this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Lägg till ett nytt HtmlTableLoadOption med tabellindex
            int index1 = tableLoadOptions.Add(0);

            // Kom åt HtmlTableLoadOption med Item-egenskapen
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Konfigurera tabellens laddningsalternativ
            option.TableToListObject = true;
            option.TargetSheetIndex = 1;

            // Läs in HTML-fil med de konfigurerade alternativen
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


