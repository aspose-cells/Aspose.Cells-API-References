---
title: "Classe NameCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.NameCollection. Rappresenta una raccolta di tutti gli oggetti Name nel foglio di calcolo"
type: docs
url: /it/net/aspose.cells/namecollection/
---
## NameCollection class

Rappresenta una raccolta di tutti gli oggetti [`Name`](../name/) nel foglio di calcolo.

```csharp
public class NameCollection : CollectionBase<Name>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/namecollection/item/) { get; } | Ottiene l'elemento [`Name`](../name/) all'indice specificato. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/namecollection/add/)(string) | Definisce un nuovo nome. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name, IComparer&lt;Name&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Name, IComparer&lt;Name&gt;) |  |
| [Clear](../../aspose.cells/namecollection/clear/#clear)() | Rimuove tutti i nomi definiti che non sono referenziati dalle formule e dalla fonte dati. Se il nome definito è referenziato, impostiamo solo Name.ReferTo a null e lo nascondiamo. (2 metodi) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Name) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Name[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Name&gt;) |  |
| [Filter](../../aspose.cells/namecollection/filter/)(NameScopeType, int) | Ottiene tutti i nomi definiti per ambito. |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Name&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int, int) |  |
| [Remove](../../aspose.cells/namecollection/remove/#remove)(string) | Rimuovi il nome. |
| [Remove](../../aspose.cells/namecollection/remove/#remove_1)(string[]) | Rimuovi un array di nomi |
| [RemoveAt](../../aspose.cells/namecollection/removeat/#removeat)(int) | Rimuovi il nome all'indice specifico. (2 metodi) |
| [RemoveDuplicateNames](../../aspose.cells/namecollection/removeduplicatenames/)() | Rimuovi i nomi definiti duplicati |
| [Sort](../../aspose.cells/namecollection/sort/)() | Ordina i nomi definiti. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionDemo
    {
        public static void NameCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla collezione di fogli di lavoro
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Accedi alla collezione di nomi
            NameCollection names = worksheets.Names;
            
            // Aggiungi un nuovo nome alla collezione
            int nameIndex = names.Add("MyNamedRange");
            Name name = names[nameIndex];
            
            // Imposta la proprietà refers to per il nome
            name.RefersTo = "=Sheet1!$A$1:$A$10";
            
            // Accedi e modifica le proprietà del nome
            name.Comment = "This is a named range for demonstration.";
            name.IsVisible = true;
            
            // Aggiungi un altro nome
            int anotherNameIndex = names.Add("AnotherNamedRange");
            Name anotherName = names[anotherNameIndex];
            anotherName.RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Rimuovi un nome per testo
            names.Remove("AnotherNamedRange");
            
            // Rimuovi un nome per indice
            names.RemoveAt(nameIndex);
            
            // Cancella tutti i nomi
            names.Clear();
            
            // Salva la cartella di lavoro
            workbook.Save("NameCollectionExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Name](../name/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


