---
title: "CustomDocumentPropertyCollection.AddLinkToContent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomDocumentPropertyCollection-metod. Skapar en ny anpassad dokumentegenskap som länkar till innehåll"
type: docs
url: /sv/net/aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/
---
## CustomDocumentPropertyCollection.AddLinkToContent method

Skapar en ny anpassad dokumentegenskap som länkar till innehåll.

```csharp
public DocumentProperty AddLinkToContent(string name, string source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på egenskapen. |
| källa | String | Källan för egenskapen. Det bör vara namnet på det namngivna området. |

### Returvärde

Det nyss skapade egenskapsobjektet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddLinkToContentWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange ett värde i cell A1 som kommer att länkas
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Lägg till en vanlig egenskap för jämförelse
            customProperties.Add("RegularProperty", "Static Value");
            
            // Lägg till en länkad egenskap
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");
            
            // Uppdatera det länkade värdet
            customProperties.UpdateLinkedRange();

            // Visa egenskaperna
            Console.WriteLine($"Regular Property: {customProperties["RegularProperty"].Value}");
            Console.WriteLine($"Linked Property: {customProperties["LinkedProperty"].Value}");

            workbook.Save("LinkedPropertyExample.xlsx");
        }
    }
}
```

### Se även

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


