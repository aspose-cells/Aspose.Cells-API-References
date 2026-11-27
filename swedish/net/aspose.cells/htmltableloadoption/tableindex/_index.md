---
title: "HtmlTableLoadOption.TableIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlTableLoadOption‑egenskap. Hämta eller ange index för tabellen som ska importeras från html"
type: docs
url: /sv/net/aspose.cells/htmltableloadoption/tableindex/
---
## HtmlTableLoadOption.TableIndex property

Hämta eller ange indexet för tabellen som ska importeras från HTML.

```csharp
public int TableIndex { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa HTML‑laddningsalternativ
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Konfigurera tabellinläsningsalternativet med TableIndex = 0 (första tabellen)
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };

            // Lägg till tabellinläsningsalternativet
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Läs in HTML‑fil (ersätt med faktisk sökväg)
            workbook = new Workbook("input.html", loadOptions);

            // Spara som Excel-fil
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


