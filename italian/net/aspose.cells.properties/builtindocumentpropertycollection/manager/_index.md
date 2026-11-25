---
title: "BuiltInDocumentPropertyCollection.Manager"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta la proprietà manager"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/manager/
---
## BuiltInDocumentPropertyCollection.Manager property

Ottiene o imposta la proprietà manager.

```csharp
public string Manager { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyManagerDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Imposta le proprietà principali del documento includendo Manager
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Manager = "Jane Smith"; // Demonstrating Manager property usage
            builtInProperties.Company = "Aspose";

            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertiesDemo.xlsx");

            Console.WriteLine("Workbook created with Manager property set to: " + builtInProperties.Manager);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


