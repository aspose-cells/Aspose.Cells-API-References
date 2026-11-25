---
title: "Classe CustomDocumentPropertyCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Properties.CustomDocumentPropertyCollection. Una raccolta di proprietà di documento personalizzate"
type: docs
url: /it/net/aspose.cells.properties/customdocumentpropertycollection/
---
## CustomDocumentPropertyCollection class

Una raccolta di proprietà del documento personalizzate.

```csharp
public class CustomDocumentPropertyCollection : DocumentPropertyCollection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Restituisce un oggetto [`DocumentProperty`](../documentproperty/) per indice.(Ereditato da [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Restituisce un oggetto [`DocumentProperty`](../documentproperty/) per il nome della proprietà.(Ereditato da [`DocumentPropertyCollection`](../documentpropertycollection/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add)(string, bool) | Crea una nuova proprietà di documento personalizzata del tipo di dati **PropertyType.Boolean**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_3)(string, DateTime) | Crea una nuova proprietà di documento personalizzata del tipo di dati **PropertyType.DateTime**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_1)(string, double) | Crea una nuova proprietà di documento personalizzata del tipo di dati **PropertyType.Float**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_2)(string, int) | Crea una nuova proprietà di documento personalizzata del tipo di dati **PropertyType.Number**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_4)(string, string) | Crea una nuova proprietà di documento personalizzata del tipo di dati **PropertyType.String**. |
| [AddLinkToContent](../../aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/)(string, string) | Crea una nuova proprietà di documento personalizzata che collega al contenuto. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DocumentProperty) |  |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains/)(string) | Restituisce true se una proprietà con il nome specificato esiste nella collezione.(Ereditato da [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DocumentProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DocumentProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty) |  |
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof/)(string) | Ottiene l'indice di una proprietà per nome.(Ereditato da [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int, int) |  |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove/)(string) | Rimuove una proprietà con il nome specificato dalla collezione.(Ereditato da [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat/)(int) | Rimuove una proprietà all'indice specificato. (2 metodi) |
| [UpdateLinkedPropertyValue](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/)() | Aggiorna i valori di tutte le proprietà personalizzate collegate al contenuto(use il valore della cella dell'intervallo collegato per aggiornare il valore della proprietà personalizzata). |
| [UpdateLinkedRange](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/)() | Aggiorna tutti gli intervalli collegati alle proprietà personalizzate(use il valore della proprietà di documento personalizzata per aggiornare il valore della cella dell'intervallo collegato). |

### Osservazioni

Ogni oggetto [`DocumentProperty`](../documentproperty/) rappresenta una proprietà personalizzata di un documento contenitore.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomDocumentPropertyCollectionDemo
    {
        public static void CustomDocumentPropertyCollectionExample()
        {
            // Istanzia un oggetto Workbook
            Workbook workbook = new Workbook();

            // Recupera un elenco di tutte le proprietà personalizzate del documento Excel
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Aggiungi proprietà di documento personalizzate
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Revision", 3);
            customProperties.Add("LastModified", DateTime.Now);
            customProperties.Add("IsFinal", true);
            customProperties.Add("Rating", 4.5);

            // Aggiungi una proprietà di documento personalizzata collegata
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");

            // Aggiorna i valori delle proprietà collegate
            //customProperties.UpdateLinkedPropertyValue();
            customProperties.UpdateLinkedRange();

            // Accesso alle proprietà di documento personalizzate
            DocumentProperty authorProperty = customProperties["Author"];
            DocumentProperty revisionProperty = customProperties["Revision"];
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DocumentProperty isFinalProperty = customProperties["IsFinal"];
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty linkedProperty = customProperties["LinkedProperty"];

            // Stampa le proprietà di documento personalizzate
            Console.WriteLine($"Author: {authorProperty.Value}");
            Console.WriteLine($"Revision: {revisionProperty.ToInt()}");
            Console.WriteLine($"Last Modified: {lastModifiedProperty.ToDateTime()}");
            Console.WriteLine($"Is Final: {isFinalProperty.ToBool()}");
            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Linked Property: {linkedProperty.Value}");

            // Salva la cartella di lavoro
            workbook.Save("CustomDocumentPropertiesExample.xlsx");
            workbook.Save("CustomDocumentPropertiesExample.pdf");
        }
    }
}
```

### Vedi anche

* class [DocumentPropertyCollection](../documentpropertycollection/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


