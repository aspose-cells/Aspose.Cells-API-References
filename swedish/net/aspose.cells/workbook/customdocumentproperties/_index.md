---
title: "Workbook.CustomDocumentProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Returnerar en DocumentProperty-samling som representerar alla anpassade dokumentegenskaper i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/workbook/customdocumentproperties/
---
## Workbook.CustomDocumentProperties property

Returnerar en [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) samling som representerar alla anpassade dokumentegenskaper i kalkylbladet.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till anpassade dokumentegenskaper
            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Created Date", DateTime.Now);
            workbook.CustomDocumentProperties.Add("Revision", 1);
            workbook.CustomDocumentProperties.Add("Approved", true);
            
            // Kom åt och visa de anpassade egenskaperna
            Console.WriteLine("Custom Document Properties:");
            foreach (Aspose.Cells.Properties.DocumentProperty prop in workbook.CustomDocumentProperties)
            {
                Console.WriteLine($"{prop.Name}: {prop.Value} ({prop.Type})");
            }
            
            // Spara arbetsboken
            workbook.Save("CustomDocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Se även

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


