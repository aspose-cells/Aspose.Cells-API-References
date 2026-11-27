---
title: "DocumentProperty.ToDateTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentProperty-metoden. Returnerar egenskapsvärdet som DateTime i lokal tidszon"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/todatetime/
---
## DocumentProperty.ToDateTime method

Returnerar egenskapsvärdet som DateTime i lokal tidszon.

```csharp
public DateTime ToDateTime()
```

### Anmärkningar

Kastar ett undantag om egenskapstypen inte är PropertyType.Date.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDateTimeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Hämta samling av anpassade dokumentegenskaper
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Lägg till en datum/tid-egenskap
            DateTime currentTime = DateTime.Now;
            customProperties.Add("LastModified", currentTime);

            // Hämta egenskapen och konvertera till DateTime
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DateTime retrievedTime = lastModifiedProperty.ToDateTime();

            // Skriv ut resultatet
            Console.WriteLine($"Stored DateTime: {currentTime}");
            Console.WriteLine($"Retrieved DateTime: {retrievedTime}");

            // Spara arbetsboken
            workbook.Save("DocumentPropertyDateTimeExample.xlsx");
        }
    }
}
```

### Se även

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


