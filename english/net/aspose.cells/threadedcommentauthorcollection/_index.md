---
title: Class ThreadedCommentAuthorCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ThreadedCommentAuthorCollection class. Represents all persons
type: docs
url: /net/aspose.cells/threadedcommentauthorcollection/
---
## ThreadedCommentAuthorCollection class

Represents all persons.

```csharp
public class ThreadedCommentAuthorCollection : CollectionBase<ThreadedCommentAuthor>
```

## Constructors

| Name | Description |
| --- | --- |
| [ThreadedCommentAuthorCollection](threadedcommentauthorcollection/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CurrentPerson](../../aspose.cells/threadedcommentauthorcollection/currentperson/) { get; set; } | Gets and sets the current user. |
| [Item](../../aspose.cells/threadedcommentauthorcollection/item/) { get; } | Gets the person who create threaded comments. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/threadedcommentauthorcollection/add/)(string, string, string) | Adds one thread comment person. |
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
| [IndexOf](../../aspose.cells/threadedcommentauthorcollection/indexof/#indexof)(ThreadedCommentAuthor) | Gets the index of ThreadedCommentAuthor object (2 methods) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedCommentAuthor, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedCommentAuthor, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionDemo
    {
        public static void ThreadedCommentAuthorCollectionExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the ThreadedCommentAuthorCollection
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Add a new threaded comment author
            int authorIndex = authors.Add("John Doe", "john.doe@example.com", "providerId123");

            // Retrieve the added author
            ThreadedCommentAuthor author = authors[authorIndex];

            // Set the current person
            authors.CurrentPerson = author;

            // Display the current person details
            Console.WriteLine("Current Person: " + authors.CurrentPerson.Name);

            // Save the workbook
            workbook.Save("ThreadedCommentAuthorCollectionExample.xlsx");

            return;
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ThreadedCommentAuthor](../threadedcommentauthor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


