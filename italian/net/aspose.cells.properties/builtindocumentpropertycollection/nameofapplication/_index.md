---
title: "BuiltInDocumentPropertyCollection.NameOfApplication"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta il nome dell'applicazione"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/nameofapplication/
---
## BuiltInDocumentPropertyCollection.NameOfApplication property

Ottiene o imposta il nome dell'applicazione.

```csharp
public string NameOfApplication { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyNameOfApplicationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la proprietà NameOfApplication
            workbook.BuiltInDocumentProperties.NameOfApplication = "Aspose.Cells Demo App";
            
            // Visualizza la proprietà NameOfApplication
            Console.WriteLine("Application Name: " + workbook.BuiltInDocumentProperties.NameOfApplication);
            
            // Salva la cartella di lavoro
            workbook.Save("output.ods");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


