---
title: "Klass HtmlTableLoadOption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlTableLoadOption-klass. Representerar alternativet när en tabell importeras från HTML"
type: docs
url: /sv/net/aspose.cells/htmltableloadoption/
---
## HtmlTableLoadOption class

Representerar alternativet när en tabell importeras från HTML.

```csharp
public class HtmlTableLoadOption
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [HtmlTableLoadOption](htmltableloadoption/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Id](../../aspose.cells/htmltableloadoption/id/) { get; set; } | Hämta eller ange id för tabellen som ska importeras från HTML |
| [Name](../../aspose.cells/htmltableloadoption/name/) { get; set; } | (**Obsolete.**) Hämta eller ange namnet på tabellen som ska importeras från HTML |
| [OriginalSheetIndex](../../aspose.cells/htmltableloadoption/originalsheetindex/) { get; set; } | Hämta eller ange det ursprungliga indexet för kalkylbladet i HTML. |
| [TableIndex](../../aspose.cells/htmltableloadoption/tableindex/) { get; set; } | Hämta eller ange indexet för tabellen som ska importeras från HTML. |
| [TableToListObject](../../aspose.cells/htmltableloadoption/tabletolistobject/) { get; set; } | Anger om listobjekt ska genereras från den importerade tabellen. Standardvärdet är falskt. |
| [TargetSheetIndex](../../aspose.cells/htmltableloadoption/targetsheetindex/) { get; set; } | Hämta eller ange målindexet för kalkylbladet där tabellen ska placeras. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionDemo
    {
        public static void HtmlTableLoadOptionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa en instans av HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Skapa en instans av HtmlTableLoadOption
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = "table1",
                Name = "SampleTable",
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // Lägg till HtmlTableLoadOption i HtmlLoadOptions
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Läs in HTML-filen i arbetsboken med de angivna laddningsalternativen
            workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("HtmlTableLoadOptionExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


