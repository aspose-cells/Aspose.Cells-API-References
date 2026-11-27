---
title: "CustomDocumentPropertyCollection.UpdateLinkedRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomDocumentPropertyCollection-metod. Uppdaterar alla områden som är länkade till anpassade egenskaper och använder värdet av den anpassade dokumentegenskapen för att uppdatera cellvärdet i det länkade området."
type: docs
url: /sv/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/
---
## CustomDocumentPropertyCollection.UpdateLinkedRange method

Uppdaterar alla områden som är länkade till anpassade egenskaper(use värdet av den anpassade dokumentegenskapen för att uppdatera cellvärdet i det länkade området).

```csharp
public void UpdateLinkedRange()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange ett värde i cell A1 som kommer att länkas
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Lägg till en länkad egenskap
            customProperties.AddLinkToContent("LinkedRange", "Sheet1!A1");
            
            // Uppdatera alla länkade egenskaper
            customProperties.UpdateLinkedRange();
            
            // Hämta och visa det länkade egenskapsvärdet
            DocumentProperty linkedProp = customProperties["LinkedRange"];
            Console.WriteLine($"Linked Property Value: {linkedProp.Value}");

            // Spara arbetsboken
            workbook.Save("LinkedRangeExample.xlsx");
        }
    }
}
```

### Se även

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


