---
title: "BuiltInDocumentPropertyCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Restituisce un oggetto DocumentProperty in base al nome della proprietà"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

Restituisce un oggetto [`DocumentProperty`](../../documentproperty/) in base al nome della proprietà.

```csharp
public override DocumentProperty this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome della proprietà da recuperare, senza distinzione tra maiuscole e minuscole. |

### Osservazioni

I nomi stringa delle proprietà corrispondono ai nomi delle proprietà tipizzate disponibili da [`BuiltInDocumentPropertyCollection`](../).

Se richiedi una proprietà che non è presente nel documento, ma il nome della proprietà è riconosciuto come un nome integrato valido, viene creata una nuova [`DocumentProperty`](../../documentproperty/), aggiunta alla collezione e restituita. Alla proprietà appena creata viene assegnato un valore predefinito (stringa vuota, zero, false o DateTime.MinValue a seconda del tipo della proprietà integrata).

Se richiedi una proprietà che non è presente nel documento e il nome non è riconosciuto come un nome integrato, viene restituito null.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta una proprietà del documento integrata usando il metodo corretto
            workbook.BuiltInDocumentProperties["Version"].Value = "15.0300";
            
            // Accedi e stampa il valore della proprietà
            Console.WriteLine("Version: " + workbook.BuiltInDocumentProperties["Version"].Value);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Carica la cartella di lavoro salvata e verifica la proprietà
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Version: " + loadedWorkbook.BuiltInDocumentProperties["Version"].Value);
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


