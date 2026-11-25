---
title: "DataModelRelationshipCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataModelRelationshipCollection. Ottiene la relazione"
type: docs
url: /it/net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

Ottiene la relazione.

```csharp
public DataModelRelationship this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro (modello dati vuoto)
            Workbook workbook = new Workbook();

            try
            {
                // Recupera la DataModelRelationshipCollection dalla cartella di lavoro (può essere null se non esiste un modello dati)
                DataModelRelationshipCollection relationships = workbook.DataModel?.Relationships;

                if (relationships == null)
                {
                    Console.WriteLine("The workbook does not contain a data model.");
                }
                else if (relationships.Count == 0)
                {
                    Console.WriteLine("The data model exists but contains no relationships.");
                }
                else
                {
                    // Leggi la prima relazione usando la proprietà Item (indicizzatore)
                    DataModelRelationship firstRelationship = relationships[0]; // Item property getter
                    Console.WriteLine("First relationship retrieved via Item property:");
                    Console.WriteLine(firstRelationship);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while accessing Item property: {ex.Message}");
            }

            // Salva la cartella di lavoro (opzionale, solo per dimostrare che il codice viene eseguito end‑to‑end)
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


