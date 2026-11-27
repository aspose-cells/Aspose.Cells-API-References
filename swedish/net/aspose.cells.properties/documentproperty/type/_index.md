---
title: "DocumentProperty.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentProperty egenskap. Hämtar datatypen för egenskapen"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/type/
---
## DocumentProperty.Type property

Hämtar datatypen för egenskapen.

```csharp
public PropertyType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till anpassade dokumentegenskaper (inte inbyggda)
            CustomDocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Lägg till anpassade egenskaper med olika typer
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 5);
            properties.Add("IsApproved", true);
            
            // Demonstrera användning av Type-egenskapen
            Console.WriteLine("Document Properties and Their Types:");
            foreach (DocumentProperty prop in properties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}, Type: {prop.Type}");
            }
            
            // Åtkomst till specifik egenskap och kontrollera dess typ
            DocumentProperty dateProp = properties["CreatedDate"];
            if (dateProp.Type == PropertyType.DateTime)
            {
                Console.WriteLine("\nCreatedDate is a DateTime property");
                Console.WriteLine($"Value as DateTime: {dateProp.ToDateTime()}");
            }
        }
    }
}
```

### Se även

* enum [PropertyType](../../propertytype/)
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


