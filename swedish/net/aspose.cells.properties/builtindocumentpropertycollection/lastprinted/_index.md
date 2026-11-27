---
title: "BuiltInDocumentPropertyCollection.LastPrinted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger datumet då dokumentet senast skrevs ut i lokal tidszon"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinted/
---
## BuiltInDocumentPropertyCollection.LastPrinted property

Hämtar eller anger datumet då dokumentet senast skrevs ut i lokal tidszon.

```csharp
public DateTime LastPrinted { get; set; }
```

### Anmärkningar

Om dokumentet aldrig har skrivits ut kommer denna egenskap att returnera DateTime.MinValue.

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in inbyggda dokumentegenskaper
            workbook.BuiltInDocumentProperties.CreatedTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now.AddDays(-1); // Set to yesterday
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Visa LastPrinted-egenskapen
            Console.WriteLine("Last printed: " + workbook.BuiltInDocumentProperties.LastPrinted);

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


