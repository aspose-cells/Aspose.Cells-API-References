---
title: "HtmlTableLoadOption.TableToListObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlTableLoadOption‑egenskap. Anger om listobjekt ska genereras från importerad tabell. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmltableloadoption/tabletolistobject/
---
## HtmlTableLoadOption.TableToListObject property

Anger om listobjekt ska genereras från den importerade tabellen. Standardvärdet är falskt.

```csharp
public bool TableToListObject { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa HTML‑inläsningsalternativ med TableToListObject aktiverat
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Läs in HTML med de angivna alternativen
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


