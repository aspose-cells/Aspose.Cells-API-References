---
title: "BuiltInDocumentPropertyCollection.TotalEditingTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta il tempo totale di modifica in minuti"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/totaleditingtime/
---
## BuiltInDocumentPropertyCollection.TotalEditingTime property

Ottiene o imposta il tempo totale di modifica in minuti.

```csharp
public double TotalEditingTime { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTotalEditingTimeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Imposta il tempo totale di modifica in minuti
            builtInProperties.TotalEditingTime = 90.5;

            // Visualizza il tempo di modifica impostato
            Console.WriteLine("Total Editing Time: " + builtInProperties.TotalEditingTime + " minutes");

            // Salva la cartella di lavoro
            workbook.Save("TotalEditingTimeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


