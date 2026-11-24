---
title: "Klasse ThreadedCommentAuthorCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ThreadedCommentAuthorCollection-Klasse. Stellt alle Personen dar"
type: docs
url: /de/net/aspose.cells/threadedcommentauthorcollection/
---
## ThreadedCommentAuthorCollection class

Stellt alle Personen dar.

```csharp
public class ThreadedCommentAuthorCollection : CollectionBase<ThreadedCommentAuthor>
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ThreadedCommentAuthorCollection](threadedcommentauthorcollection/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CurrentPerson](../../aspose.cells/threadedcommentauthorcollection/currentperson/) { get; set; } | Liest und setzt den aktuellen Benutzer. |
| [Item](../../aspose.cells/threadedcommentauthorcollection/item/) { get; } | Liest die Person, die Thread‑Kommentare erstellt. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/threadedcommentauthorcollection/add/)(string, string, string) | Fügt eine Thread‑Kommentar‑Person hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ThreadedCommentAuthor) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ThreadedCommentAuthor, IComparer&lt;ThreadedCommentAuthor&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ThreadedCommentAuthor, IComparer&lt;ThreadedCommentAuthor&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ThreadedCommentAuthor) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ThreadedCommentAuthor[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ThreadedCommentAuthor[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ThreadedCommentAuthor[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/threadedcommentauthorcollection/indexof/#indexof)(ThreadedCommentAuthor) | Liest den Index des ThreadedCommentAuthor‑Objekts (2 Methoden) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedCommentAuthor, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedCommentAuthor, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionDemo
    {
        public static void ThreadedCommentAuthorCollectionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die ThreadedCommentAuthorCollection
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Fügen Sie einen neuen Thread‑Kommentar‑Autor hinzu
            int authorIndex = authors.Add("John Doe", "john.doe@example.com", "providerId123");

            // Den hinzugefügten Autor abrufen
            ThreadedCommentAuthor author = authors[authorIndex];

            // Setzen Sie die aktuelle Person
            authors.CurrentPerson = author;

            // Zeigen Sie die Details der aktuellen Person an
            Console.WriteLine("Current Person: " + authors.CurrentPerson.Name);

            // Speichere die Arbeitsmappe
            workbook.Save("ThreadedCommentAuthorCollectionExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ThreadedCommentAuthor](../threadedcommentauthor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


