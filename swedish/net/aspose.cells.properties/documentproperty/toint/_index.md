---
title: "DocumentProperty.ToInt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentProperty‑metod. Returnerar egenskapsvärdet som heltal"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/toint/
---
## DocumentProperty.ToInt method

Returnerar egenskapsvärdet som integer.

```csharp
public int ToInt()
```

### Anmärkningar

Kastar ett undantag om egenskapstypen inte är PropertyType.Number.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToIntDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Hämta samlingen av anpassade dokumentegenskaper
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Lägg till en numerisk anpassad egenskap
            customProperties.Add("Revision", 5);

            // Hämta egenskapen och konvertera till int med ToInt()
            DocumentProperty revisionProperty = customProperties["Revision"];
            int revisionValue = revisionProperty.ToInt();
            
            // Skriv ut resultatet
            Console.WriteLine($"Revision (as int): {revisionValue}");

            // Spara arbetsboken
            workbook.Save("DocumentPropertyToIntExample.xlsx");
        }
    }
}
```

### Se även

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


