---
title: "DocumentProperty.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentProperty-egenskapen. Returnerar namnet på egenskapen"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/name/
---
## DocumentProperty.Name property

Returnerar egenskapens namn.

```csharp
public string Name { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Få åtkomst till dokumentegenskaper
            BuiltInDocumentPropertyCollection builtInProps = workbook.BuiltInDocumentProperties;
            CustomDocumentPropertyCollection customProps = workbook.CustomDocumentProperties;
            
            // Lägg till en anpassad egenskap och demonstrera användning av Name
            DocumentProperty authorProperty = customProps.Add("Author", "John Doe");
            Console.WriteLine("Property Name: " + authorProperty.Name);
            Console.WriteLine("Property Value: " + authorProperty.Value);
            
            // Få åtkomst till en inbyggd egenskap med namn
            DocumentProperty titleProperty = builtInProps["Title"];
            titleProperty.Value = "Sample Document";
            Console.WriteLine("Title Property Name: " + titleProperty.Name);
            Console.WriteLine("Title Property Value: " + titleProperty.Value);
        }
    }
}
```

### Se även

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


