---
title: "BuiltInDocumentPropertyCollection.CreatedTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger datum för dokumentets skapande i lokal tidszon"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/createdtime/
---
## BuiltInDocumentPropertyCollection.CreatedTime property

Hämtar eller anger datum för dokumentets skapande i lokal tidszon.

```csharp
public DateTime CreatedTime { get; set; }
```

### Anmärkningar

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in CreatedTime-egenskapen till aktuell tid
            DateTime currentTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.CreatedTime = currentTime;
            
            // Spara arbetsboken
            string outputPath = "output_CreatedTimeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Läs in den sparade arbetsboken för att verifiera egenskapen
            Workbook loadedWorkbook = new Workbook(outputPath);
            DateTime loadedTime = loadedWorkbook.BuiltInDocumentProperties.CreatedTime;
            
            Console.WriteLine("Original CreatedTime: " + currentTime);
            Console.WriteLine("Loaded CreatedTime: " + loadedTime);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


