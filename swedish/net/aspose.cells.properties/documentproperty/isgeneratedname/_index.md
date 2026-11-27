---
title: "DocumentProperty.IsGeneratedName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentProperty‑egenskap. Returnerar true om denna egenskap inte har ett namn i OLE2‑lagringen och ett unikt namn genererades endast för det offentliga API:et"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/isgeneratedname/
---
## DocumentProperty.IsGeneratedName property

Returnerar true om denna egenskap inte har ett namn i OLE2-lagringen och ett unikt namn genererades endast för det offentliga API:et.

```csharp
public bool IsGeneratedName { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyPropertyIsGeneratedNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till inbyggda dokumentegenskaper
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;
            
            // Åtkomst till anpassade dokumentegenskaper för att lägga till
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Lägg till en anpassad egenskap
            DocumentProperty customProperty = customProperties.Add("CustomProperty", "Test Value");
            
            // Visa IsGeneratedName för inbyggd egenskap
            DocumentProperty authorProperty = properties["Author"];
            Console.WriteLine("Author property IsGeneratedName: " + authorProperty.IsGeneratedName);
            
            // Visa IsGeneratedName för anpassad egenskap
            Console.WriteLine("Custom property IsGeneratedName: " + customProperty.IsGeneratedName);

            // Skapa ett scenario där en egenskap kan ha ett genererat namn
            // (Obs: I praktiken är IsGeneratedName skrivskyddad och sätts internt av Aspose.Cells)
            DocumentProperty generatedNameProperty = properties["_PID_GUID"];
            if (generatedNameProperty != null)
            {
                Console.WriteLine("Generated name property IsGeneratedName: " + generatedNameProperty.IsGeneratedName);
            }

            // Spara arbetsboken
            workbook.Save("PropertyIsGeneratedNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


