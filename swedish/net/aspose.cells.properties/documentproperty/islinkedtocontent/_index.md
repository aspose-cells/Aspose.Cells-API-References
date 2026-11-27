---
title: "DocumentProperty.IsLinkedToContent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentProperty-egenskapen. Anger om denna egenskap är länkad till innehåll"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/islinkedtocontent/
---
## DocumentProperty.IsLinkedToContent property

Indikerar om denna egenskap är länkad till innehåll

```csharp
public bool IsLinkedToContent { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyIsLinkedToContentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata i celler
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Company Name";
            worksheet.Cells["B1"].Value = "Company Address";

            // Skapa länkade anpassade dokumentegenskaper
            workbook.CustomDocumentProperties.AddLinkToContent("Company", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Address", "B1");

            // Hämta och kontrollera IsLinkedToContent-egenskapen
            DocumentProperty companyProp = workbook.CustomDocumentProperties["Company"];
            Console.WriteLine($"Is 'Company' property linked to content: {companyProp.IsLinkedToContent}");
            Console.WriteLine($"Linked source: {companyProp.Source}");
            Console.WriteLine($"Current value: {companyProp.Value}");

            // Uppdatera cellvärdet och uppdatera länkade egenskaper
            worksheet.Cells["A1"].Value = "Updated Company Name";
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Verifiera att egenskapen uppdaterades
            Console.WriteLine($"Updated value: {companyProp.Value}");

            // Spara arbetsboken
            workbook.Save("LinkedPropertiesDemo.xlsx");
        }
    }
}
```

### Se även

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


