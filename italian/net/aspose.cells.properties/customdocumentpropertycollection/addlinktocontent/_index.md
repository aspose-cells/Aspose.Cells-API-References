---
title: "CustomDocumentPropertyCollection.AddLinkToContent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomDocumentPropertyCollection. Crea una nuova proprietà documento personalizzata che si collega al contenuto"
type: docs
url: /it/net/aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/
---
## CustomDocumentPropertyCollection.AddLinkToContent method

Crea una nuova proprietà di documento personalizzata che collega al contenuto.

```csharp
public DocumentProperty AddLinkToContent(string name, string source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà. |
| origine | String | L'origine della proprietà. Deve essere il nome dell'intervallo denominato. |

### Valore di ritorno

L'oggetto proprietà appena creato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddLinkToContentWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta un valore nella cella A1 che sarà collegato
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Aggiungi una proprietà regolare per confronto
            customProperties.Add("RegularProperty", "Static Value");
            
            // Aggiungi una proprietà collegata
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");
            
            // Aggiorna il valore collegato
            customProperties.UpdateLinkedRange();

            // Visualizza le proprietà
            Console.WriteLine($"Regular Property: {customProperties["RegularProperty"].Value}");
            Console.WriteLine($"Linked Property: {customProperties["LinkedProperty"].Value}");

            workbook.Save("LinkedPropertyExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


