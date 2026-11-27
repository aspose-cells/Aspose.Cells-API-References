---
title: "DocumentProperty.ToDouble"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentProperty-metoden. Returnerar egenskapsvärdet som double"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/todouble/
---
## DocumentProperty.ToDouble method

Returnerar egenskapsvärdet som double.

```csharp
public double ToDouble()
```

### Anmärkningar

Kastar ett undantag om egenskapstypen inte är PropertyType.Float.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDoubleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Hämta samling av anpassade dokumentegenskaper
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Lägg till en numerisk egenskap
            customProperties.Add("Rating", 4.75);

            // Hämta egenskapen och konvertera till double
            DocumentProperty ratingProperty = customProperties["Rating"];
            double ratingValue = ratingProperty.ToDouble();

            // Skriv ut resultatet
            Console.WriteLine($"Rating: {ratingValue}");

            // Spara arbetsboken
            workbook.Save("DocumentPropertyToDoubleExample.xlsx");
        }
    }
}
```

### Se även

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


