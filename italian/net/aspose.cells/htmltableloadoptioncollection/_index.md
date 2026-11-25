---
title: "Classe HtmlTableLoadOptionCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.HtmlTableLoadOptionCollection. Rappresenta le opzioni della tabella durante l'importazione di HTML"
type: docs
url: /it/net/aspose.cells/htmltableloadoptioncollection/
---
## HtmlTableLoadOptionCollection class

Rappresenta le opzioni della tabella durante l'importazione di HTML.

```csharp
public class HtmlTableLoadOptionCollection : CollectionBase<HtmlTableLoadOption>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [HtmlTableLoadOptionCollection](htmltableloadoptioncollection/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/htmltableloadoptioncollection/item/) { get; } | Ottiene l'elemento [`HtmlTableLoadOption`](../htmltableloadoption/) all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [TableToListObject](../../aspose.cells/htmltableloadoptioncollection/tabletolistobject/) { get; set; } | Indica se generare oggetti elenco dalle tabelle importate. Il valore predefinito è false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add)(HtmlTableLoadOption) | (**Obsoleto.**) Aggiunge un HtmlTableLoadOption a questa collezione. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_1)(int) | Aggiungi un HtmlTableLoadOption all'elenco. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_4)(string) | Aggiungi un HtmlTableLoadOption all'elenco. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_2)(int, int) | Aggiungi un HtmlTableLoadOption all'elenco. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_5)(string, int) | Aggiungi un HtmlTableLoadOption all'elenco. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_3)(int, int, int) | Aggiungi un HtmlTableLoadOption all'elenco. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_6)(string, int, int) | Aggiungi un HtmlTableLoadOption all'elenco. |
| [AddTableLoadOption](../../aspose.cells/htmltableloadoptioncollection/addtableloadoption/)(HtmlTableLoadOption) | Aggiunge un HtmlTableLoadOption a questa collezione. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HtmlTableLoadOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HtmlTableLoadOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionCollectionDemo
    {
        public static void HtmlTableLoadOptionCollectionExample()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();

            // Crea HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accedi all'istanza di HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Imposta la proprietà TableToListObject
            tableLoadOptions.TableToListObject = true;

            // Aggiungi una nuova HtmlTableLoadOption per indice tabella
            int index1 = tableLoadOptions.Add(0);

            // Aggiungi una nuova HtmlTableLoadOption per ID tabella
            int index2 = tableLoadOptions.Add("tableId");

            // Aggiungi una nuova HtmlTableLoadOption per indice tabella e indice foglio di destinazione
            int index3 = tableLoadOptions.Add(1, 1);

            // Aggiungi una nuova HtmlTableLoadOption per ID tabella e indice foglio di destinazione
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Aggiungi una nuova HtmlTableLoadOption per indice tabella, indice foglio di destinazione e indice foglio originale
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Aggiungi una nuova HtmlTableLoadOption per ID tabella, indice foglio di destinazione e indice foglio originale
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Accedi alla HtmlTableLoadOption a un indice specifico
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Imposta le proprietà della HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Carica un file HTML nella cartella di lavoro usando le opzioni di caricamento
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Salva la cartella di lavoro
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HtmlTableLoadOption](../htmltableloadoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


