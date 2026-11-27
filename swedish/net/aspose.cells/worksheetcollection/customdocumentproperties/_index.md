---
title: "WorksheetCollection.CustomDocumentProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Returnerar en DocumentProperty-samling som representerar alla anpassade dokumentegenskaper i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/customdocumentproperties/
---
## WorksheetCollection.CustomDocumentProperties property

Returnerar en [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) samling som representerar alla anpassade dokumentegenskaper i kalkylbladet.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till anpassade dokumentegenskaper
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("CreatedDate", DateTime.Now);
            workbook.Worksheets.CustomDocumentProperties.Add("Version", 1.2);
            
            // Åtkomst och visa egenskaperna
            Console.WriteLine("Author: " + workbook.Worksheets.CustomDocumentProperties["Author"]);
            Console.WriteLine("Created: " + workbook.Worksheets.CustomDocumentProperties["CreatedDate"]);
            Console.WriteLine("Version: " + workbook.Worksheets.CustomDocumentProperties["Version"]);
        }
    }
}
```

### Se även

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


