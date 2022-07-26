---
title: HyperlinkCollection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula una raccolta diHyperlink./hyperlink oggetti.
type: docs
weight: 3760
url: /it/net/aspose.cells/hyperlinkcollection/
---
## HyperlinkCollection class

Incapsula una raccolta di[`Hyperlink`](../hyperlink) oggetti.

```csharp
public class HyperlinkCollection : CollectionBase<Hyperlink>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/hyperlinkcollection/item) { get; } | Ottiene il[`Hyperlink`](../hyperlink) elemento all'indice specificato. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/hyperlinkcollection/add#add_1)(string, int, int, string) | Aggiunge un collegamento ipertestuale a una cella specificata oa un intervallo di celle. |
| [Add](../../aspose.cells/hyperlinkcollection/add#add)(int, int, int, int, string) | Aggiunge un collegamento ipertestuale a una cella specificata oa un intervallo di celle. |
| [Add](../../aspose.cells/hyperlinkcollection/add#add_2)(string, string, string, string, string) | Aggiunge un collegamento ipertestuale a una cella specificata oa un intervallo di celle. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Hyperlink) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [Clear](../../aspose.cells/hyperlinkcollection/clear#clear)() | Cancella tutti i collegamenti ipertestuali. (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Hyperlink) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Hyperlink[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Hyperlink[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Hyperlink[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Hyperlink&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Hyperlink&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Hyperlink) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Hyperlink, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Hyperlink, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Hyperlink) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Hyperlink, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Hyperlink, int, int) |  |
| [RemoveAt](../../aspose.cells/hyperlinkcollection/removeat#removeat)(int) | Rimuovere il collegamento ipertestuale all'indice specificato. (2 methods) |

### Esempi

```csharp


[C#]

//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();

//Ottenere il riferimento del foglio di lavoro appena aggiunto passando il relativo indice del foglio
Worksheet worksheet = workbook.Worksheets[0];

//Ottieni la raccolta di collegamenti ipertestuali
HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

//Aggiunta di un collegamento ipertestuale a un URL nella cella "A1".
hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

//Salvataggio del file Excel
workbook.Save("book1.xls");

[VB.NET]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()

'Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice del foglio
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Ottieni la raccolta di collegamenti ipertestuali
Dim hyperlinks As HyperlinkCollection = worksheet.Hyperlinks

'Adding a hyperlink to a URL at "A1" cell
hyperlinks.Add("A1", 1, 1, "http://www.aspose.com")

'Salvataggio del file Excel
workbook.Save("book1.xls")
```

### Guarda anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Hyperlink](../hyperlink)
* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
