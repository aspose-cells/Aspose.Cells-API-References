---
title: "CustomDocumentPropertyCollection.UpdateLinkedPropertyValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomDocumentPropertyCollection-metod. Uppdaterar värden för alla anpassade egenskaper som är länkade till innehållsanvänd cellvärde i den länkade raden för att uppdatera värdet på den anpassade egenskapen."
type: docs
url: /sv/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/
---
## CustomDocumentPropertyCollection.UpdateLinkedPropertyValue method

Uppdaterar värden för alla anpassade egenskaper som är länkade till innehåll(use cellvärdet i det länkade området för att uppdatera värdet för den anpassade egenskapen).

```csharp
public void UpdateLinkedPropertyValue()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till lite data i celler som kommer att länkas till anpassade egenskaper
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "InitialValue1";
            worksheet.Cells["B1"].Value = "InitialValue2";

            // Lägg till länkade anpassade egenskaper
            workbook.CustomDocumentProperties.AddLinkToContent("CompanyName", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Department", "B1");

            // Uppdatera cellvärdena
            worksheet.Cells["A1"].Value = "UpdatedValue1";
            worksheet.Cells["B1"].Value = "UpdatedValue2";

            // Uppdatera de länkade egenskapsvärdena
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Visa de uppdaterade egenskapsvärdena
            Console.WriteLine("CompanyName: " + workbook.CustomDocumentProperties["CompanyName"].Value);
            Console.WriteLine("Department: " + workbook.CustomDocumentProperties["Department"].Value);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


