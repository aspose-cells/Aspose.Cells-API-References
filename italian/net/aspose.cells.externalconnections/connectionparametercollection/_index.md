---
title: "Classe ConnectionParameterCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ExternalConnections.ConnectionParameterCollection. Specifica la raccolta ConnectionParameter"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparametercollection/
---
## ConnectionParameterCollection class

Specifica la raccolta [`ConnectionParameter`](../connectionparameter/)

```csharp
public class ConnectionParameterCollection : CollectionBase<ConnectionParameter>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.externalconnections/connectionparametercollection/item/) { get; } | Ottiene l'elemento [`ConnectionParameter`](../connectionparameter/) all'indice specificato. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConnectionParameter) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConnectionParameter, IComparer&lt;ConnectionParameter&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ConnectionParameter, IComparer&lt;ConnectionParameter&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ConnectionParameter) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConnectionParameter[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConnectionParameter[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ConnectionParameter[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ConnectionParameter&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterCollectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            
            try
            {
                // Ottieni la prima connessione esterna (ne verrà creata una se non esiste)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Ottieni la raccolta dei parametri dalla connessione
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Dimostra la funzionalità di base verificando le proprietà della raccolta
                Console.WriteLine($"ConnectionParameterCollection count: {parameters.Count}");
                
                // Prova ad accedere a un elemento (sarà null se la raccolta è vuota)
                if (parameters.Count > 0)
                {
                    ConnectionParameter param = parameters[0];
                    Console.WriteLine(param == null ? "No parameters in collection" : "Parameter exists");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterCollectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameterCollection: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ConnectionParameter](../connectionparameter/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


