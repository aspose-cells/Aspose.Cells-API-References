---
title: "BuiltInDocumentPropertyCollection.LastPrinted"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta la data in cui il documento è stato stampato l'ultima volta nel fuso orario locale"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinted/
---
## BuiltInDocumentPropertyCollection.LastPrinted property

Ottiene o imposta la data in cui il documento è stato stampato l'ultima volta nel fuso orario locale.

```csharp
public DateTime LastPrinted { get; set; }
```

### Osservazioni

Se il documento non è mai stato stampato, questa proprietà restituirà DateTime.MinValue.

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta le proprietà integrate del documento
            workbook.BuiltInDocumentProperties.CreatedTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now.AddDays(-1); // Set to yesterday
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Visualizza la proprietà LastPrinted
            Console.WriteLine("Last printed: " + workbook.BuiltInDocumentProperties.LastPrinted);

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


