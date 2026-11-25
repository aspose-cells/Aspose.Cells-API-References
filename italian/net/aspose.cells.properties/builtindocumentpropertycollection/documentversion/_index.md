---
title: "BuiltInDocumentPropertyCollection.DocumentVersion"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Rappresenta la versione del file"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/documentversion/
---
## BuiltInDocumentPropertyCollection.DocumentVersion property

Rappresenta la versione del file.

```csharp
public string DocumentVersion { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyDocumentVersionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la proprietà della versione del documento
            workbook.BuiltInDocumentProperties.DocumentVersion = "1.0";
            
            // Visualizza la versione del documento
            Console.WriteLine("Document Version: " + workbook.BuiltInDocumentProperties.DocumentVersion);
            
            // Salva la cartella di lavoro
            workbook.Save("DocumentVersionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


