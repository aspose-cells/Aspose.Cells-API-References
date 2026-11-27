---
title: "HtmlTableLoadOptionCollection.TableToListObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlTableLoadOptionCollection-egenskap. Anger om listobjekt ska genereras från importerade tabeller. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmltableloadoptioncollection/tabletolistobject/
---
## HtmlTableLoadOptionCollection.TableToListObject property

Anger om listobjekt ska genereras från importerade tabeller. Standardvärdet är false.

```csharp
public bool TableToListObject { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Kom åt HtmlTableLoadOptionCollection-instansen
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Ställ in TableToListObject-egenskapen för att konvertera HTML-tabeller till ListObjects
            tableLoadOptions.TableToListObject = true;

            // Lägg till en tabell som ska konverteras till ListObject efter index
            tableLoadOptions.Add(0);

            // Läs in en HTML-fil i arbetsboken med hjälp av laddningsalternativen
            workbook = new Workbook("input.html", loadOptions);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


