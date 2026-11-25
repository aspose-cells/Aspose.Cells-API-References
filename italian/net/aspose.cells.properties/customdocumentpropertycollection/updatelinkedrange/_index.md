---
title: "CustomDocumentPropertyCollection.UpdateLinkedRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CustomDocumentPropertyCollection metodo. Aggiorna tutti gli intervalli collegati a proprietà personalizzate usando il valore della proprietà del documento personalizzato per aggiornare il valore della cella dell'intervallo collegato"
type: docs
url: /it/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/
---
## CustomDocumentPropertyCollection.UpdateLinkedRange method

Aggiorna tutti gli intervalli collegati alle proprietà personalizzate(use il valore della proprietà di documento personalizzata per aggiornare il valore della cella dell'intervallo collegato).

```csharp
public void UpdateLinkedRange()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta un valore nella cella A1 che sarà collegato
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Aggiungi una proprietà collegata
            customProperties.AddLinkToContent("LinkedRange", "Sheet1!A1");
            
            // Aggiorna tutte le proprietà collegate
            customProperties.UpdateLinkedRange();
            
            // Ottieni e visualizza il valore della proprietà collegata
            DocumentProperty linkedProp = customProperties["LinkedRange"];
            Console.WriteLine($"Linked Property Value: {linkedProp.Value}");

            // Salva la cartella di lavoro
            workbook.Save("LinkedRangeExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


