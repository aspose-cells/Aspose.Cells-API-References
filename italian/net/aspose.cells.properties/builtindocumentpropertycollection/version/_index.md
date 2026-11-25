---
title: "BuiltInDocumentPropertyCollection.Version"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Rappresenta il numero di versione dell'applicazione che ha creato il documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/version/
---
## BuiltInDocumentPropertyCollection.Version property

Rappresenta il numero di versione dell'applicazione che ha creato il documento.

```csharp
public string Version { get; set; }
```

### Osservazioni

Il suo formato è "00.0000", per esempio: 12.0000

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyVersionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta alcune proprietà del documento
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Accedi e visualizza la proprietà Version
            string version = workbook.BuiltInDocumentProperties.Version;
            Console.WriteLine("Document Version: " + version);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


