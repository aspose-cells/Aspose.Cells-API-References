---
title: "BuiltInDocumentPropertyCollection.CreatedUniversalTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger den universella tiden för dokumentets skapande"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/createduniversaltime/
---
## BuiltInDocumentPropertyCollection.CreatedUniversalTime property

Hämtar eller anger den universella tiden för dokumentets skapande.

```csharp
public DateTime CreatedUniversalTime { get; set; }
```

### Anmärkningar

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCreatedUniversalTimeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ange CreatedUniversalTime-egenskapen
            DateTime creationTime = new DateTime(2023, 5, 15, 15, 30, 0, DateTimeKind.Utc);
            workbook.BuiltInDocumentProperties.CreatedUniversalTime = creationTime;
            
            // Visa CreatedUniversalTime-egenskapen
            Console.WriteLine("Document created (UTC): " + 
                workbook.BuiltInDocumentProperties.CreatedUniversalTime.ToString());
            
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


