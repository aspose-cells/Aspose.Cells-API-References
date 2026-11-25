---
title: "Workbook.CustomDocumentProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Restituisce una raccolta DocumentProperty che rappresenta tutte le proprietà documento personalizzate del foglio di calcolo"
type: docs
url: /it/net/aspose.cells/workbook/customdocumentproperties/
---
## Workbook.CustomDocumentProperties property

Restituisce una raccolta di [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà personalizzate del documento del foglio di calcolo.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi proprietà di documento personalizzate
            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Created Date", DateTime.Now);
            workbook.CustomDocumentProperties.Add("Revision", 1);
            workbook.CustomDocumentProperties.Add("Approved", true);
            
            // Accedi e visualizza le proprietà personalizzate
            Console.WriteLine("Custom Document Properties:");
            foreach (Aspose.Cells.Properties.DocumentProperty prop in workbook.CustomDocumentProperties)
            {
                Console.WriteLine($"{prop.Name}: {prop.Value} ({prop.Type})");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("CustomDocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


