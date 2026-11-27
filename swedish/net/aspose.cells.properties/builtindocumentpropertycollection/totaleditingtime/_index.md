---
title: "BuiltInDocumentPropertyCollection.TotalEditingTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger den totala redigeringstiden i minuter"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/totaleditingtime/
---
## BuiltInDocumentPropertyCollection.TotalEditingTime property

Hämtar eller anger total redigeringstid i minuter.

```csharp
public double TotalEditingTime { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTotalEditingTimeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till de inbyggda dokumentegenskaperna
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Ange den totala redigeringstiden i minuter
            builtInProperties.TotalEditingTime = 90.5;

            // Visa den angivna redigeringstiden
            Console.WriteLine("Total Editing Time: " + builtInProperties.TotalEditingTime + " minutes");

            // Spara arbetsboken
            workbook.Save("TotalEditingTimeDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


