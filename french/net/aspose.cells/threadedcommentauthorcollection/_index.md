---
title: "Class ThreadedCommentAuthorCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ThreadedCommentAuthorCollection. Représente toutes les personnes"
type: docs
url: /fr/net/aspose.cells/threadedcommentauthorcollection/
---
## ThreadedCommentAuthorCollection class

Représente toutes les personnes.

```csharp
public class ThreadedCommentAuthorCollection : CollectionBase<ThreadedCommentAuthor>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ThreadedCommentAuthorCollection](threadedcommentauthorcollection/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CurrentPerson](../../aspose.cells/threadedcommentauthorcollection/currentperson/) { get; set; } | Obtient et définit l'utilisateur actuel. |
| [Item](../../aspose.cells/threadedcommentauthorcollection/item/) { get; } | Obtient la personne qui crée les commentaires en fil. (2 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/threadedcommentauthorcollection/add/)(string, string, string) | Ajoute une personne de commentaire en fil. |
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
| [IndexOf](../../aspose.cells/threadedcommentauthorcollection/indexof/#indexof)(ThreadedCommentAuthor) | Obtient l'index de l'objet ThreadedCommentAuthor (2 méthodes) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedCommentAuthor, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedCommentAuthor, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionDemo
    {
        public static void ThreadedCommentAuthorCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la ThreadedCommentAuthorCollection
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Ajouter un nouvel auteur de commentaire en fil
            int authorIndex = authors.Add("John Doe", "john.doe@example.com", "providerId123");

            // Récupérer l'auteur ajouté
            ThreadedCommentAuthor author = authors[authorIndex];

            // Définir la personne actuelle
            authors.CurrentPerson = author;

            // Afficher les détails de la personne actuelle
            Console.WriteLine("Current Person: " + authors.CurrentPerson.Name);

            // Enregistrez le classeur
            workbook.Save("ThreadedCommentAuthorCollectionExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ThreadedCommentAuthor](../threadedcommentauthor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


