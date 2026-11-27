---
title: "DocumentProperty.Source"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentProperty egenskap. Den länkade innehållskällan"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/source/
---
## DocumentProperty.Source property

Den länkade innehållskällan.

```csharp
public string Source { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertySourceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till anpassade dokumentegenskaper
            var properties = workbook.Worksheets.CustomDocumentProperties;

            // Lägg till egenskaper
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 1);
            
            // Hämta egenskaper och visa deras källor
            Console.WriteLine("Property Sources:");
            Console.WriteLine($"Author: {properties["Author"].Source}");
            Console.WriteLine($"CreatedDate: {properties["CreatedDate"].Source}");
            Console.WriteLine($"Revision: {properties["Revision"].Source}");

            // Spara arbetsboken
            workbook.Save("DocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Se även

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


