---
title: "WorksheetCollection.CustomDocumentProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorksheetCollection. Restituisce una raccolta di DocumentProperty che rappresenta tutte le proprietà personalizzate del documento del foglio di calcolo"
type: docs
url: /it/net/aspose.cells/worksheetcollection/customdocumentproperties/
---
## WorksheetCollection.CustomDocumentProperties property

Restituisce una raccolta di [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà personalizzate del documento del foglio di calcolo.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi proprietà di documento personalizzate
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("CreatedDate", DateTime.Now);
            workbook.Worksheets.CustomDocumentProperties.Add("Version", 1.2);
            
            // Accedi e visualizza le proprietà
            Console.WriteLine("Author: " + workbook.Worksheets.CustomDocumentProperties["Author"]);
            Console.WriteLine("Created: " + workbook.Worksheets.CustomDocumentProperties["CreatedDate"]);
            Console.WriteLine("Version: " + workbook.Worksheets.CustomDocumentProperties["Version"]);
        }
    }
}
```

### Vedi anche

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


