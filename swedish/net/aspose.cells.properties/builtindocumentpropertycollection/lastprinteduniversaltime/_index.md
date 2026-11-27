---
title: "BuiltInDocumentPropertyCollection.LastPrintedUniversalTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger den universella tiden då dokumentet senast skrevs ut"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinteduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastPrintedUniversalTime property

Hämtar eller anger den universella tiden då dokumentet senast skrevs ut.

```csharp
public DateTime LastPrintedUniversalTime { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedUniversalTimeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till de inbyggda dokumentegenskaperna
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Ställ in LastPrintedUniversalTime‑egenskapen
            DateTime currentUtcTime = DateTime.UtcNow;
            builtInProperties.LastPrintedUniversalTime = currentUtcTime;

            // Visa det angivna värdet
            Console.WriteLine("LastPrintedUniversalTime set to: " + builtInProperties.LastPrintedUniversalTime);

            // Spara arbetsboken
            workbook.Save("LastPrintedUniversalTimeDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


