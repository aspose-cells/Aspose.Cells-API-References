---
title: "BuiltInDocumentPropertyCollection.LastSavedUniversalTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection property. Hämtar eller anger den universella tiden för den senaste sparningen"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/lastsaveduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastSavedUniversalTime property

Hämtar eller anger den universella tiden för den senaste sparningen.

```csharp
public DateTime LastSavedUniversalTime { get; set; }
```

### Anmärkningar

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedUniversalTimeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till de inbyggda dokumentegenskaperna
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Ange LastSavedUniversalTime‑egenskapen
            DateTime utcNow = DateTime.UtcNow;
            builtInProperties.LastSavedUniversalTime = utcNow;

            // Visa det angivna värdet
            Console.WriteLine("LastSavedUniversalTime set to: " + builtInProperties.LastSavedUniversalTime);

            // Spara arbetsboken
            workbook.Save("LastSavedUniversalTimeDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


