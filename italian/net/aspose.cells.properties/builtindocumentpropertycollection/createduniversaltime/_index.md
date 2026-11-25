---
title: "BuiltInDocumentPropertyCollection.CreatedUniversalTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta il tempo universale della creazione del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/createduniversaltime/
---
## BuiltInDocumentPropertyCollection.CreatedUniversalTime property

Ottiene o imposta l'ora universale di creazione del documento.

```csharp
public DateTime CreatedUniversalTime { get; set; }
```

### Osservazioni

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCreatedUniversalTimeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la proprietà CreatedUniversalTime
            DateTime creationTime = new DateTime(2023, 5, 15, 15, 30, 0, DateTimeKind.Utc);
            workbook.BuiltInDocumentProperties.CreatedUniversalTime = creationTime;
            
            // Visualizza la proprietà CreatedUniversalTime
            Console.WriteLine("Document created (UTC): " + 
                workbook.BuiltInDocumentProperties.CreatedUniversalTime.ToString());
            
            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


