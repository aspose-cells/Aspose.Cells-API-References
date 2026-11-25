---
title: "BuiltInDocumentPropertyCollection.LastSavedTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta l'ora dell'ultimo salvataggio nel fuso orario locale"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/lastsavedtime/
---
## BuiltInDocumentPropertyCollection.LastSavedTime property

Ottiene o imposta l'ora dell'ultimo salvataggio nel fuso orario locale.

```csharp
public DateTime LastSavedTime { get; set; }
```

### Osservazioni

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedTimeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta le proprietà integrate del documento
            workbook.BuiltInDocumentProperties.CreatedTime = new DateTime(2023, 1, 1);
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Visualizza la proprietà LastSavedTime
            Console.WriteLine("Last Saved Time: " + 
                workbook.BuiltInDocumentProperties.LastSavedTime);

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


