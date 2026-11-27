---
title: "BuiltInDocumentPropertyCollection.LastSavedTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger tiden för den senaste sparningen i lokal tidszon"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/lastsavedtime/
---
## BuiltInDocumentPropertyCollection.LastSavedTime property

Hämtar eller anger tiden för den senaste sparningen i lokal tidszon.

```csharp
public DateTime LastSavedTime { get; set; }
```

### Anmärkningar

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedTimeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in inbyggda dokumentegenskaper
            workbook.BuiltInDocumentProperties.CreatedTime = new DateTime(2023, 1, 1);
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Visa LastSavedTime-egenskapen
            Console.WriteLine("Last Saved Time: " + 
                workbook.BuiltInDocumentProperties.LastSavedTime);

            // Spara arbetsboken
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


