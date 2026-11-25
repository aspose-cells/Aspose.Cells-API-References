---
title: "BuiltInDocumentPropertyCollection.LastSavedUniversalTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta l'ora universale dell'ultimo salvataggio"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/lastsaveduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastSavedUniversalTime property

Ottiene o imposta l'ora universale dell'ultimo salvataggio.

```csharp
public DateTime LastSavedUniversalTime { get; set; }
```

### Osservazioni

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedUniversalTimeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Imposta la proprietà LastSavedUniversalTime
            DateTime utcNow = DateTime.UtcNow;
            builtInProperties.LastSavedUniversalTime = utcNow;

            // Visualizza il valore impostato
            Console.WriteLine("LastSavedUniversalTime set to: " + builtInProperties.LastSavedUniversalTime);

            // Salva la cartella di lavoro
            workbook.Save("LastSavedUniversalTimeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


