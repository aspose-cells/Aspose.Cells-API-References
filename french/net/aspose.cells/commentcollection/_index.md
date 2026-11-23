---
title: "Classe CommentCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CommentCollection. Encapsule une collection d'objets Comment"
type: docs
url: /fr/net/aspose.cells/commentcollection/
---
## CommentCollection class

Encapsule une collection d'objets [`Comment`](../comment/).

```csharp
public class CommentCollection : CollectionBase<Comment>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/commentcollection/item/) { get; } | Obtient l'élément [`Comment`](../comment/) à l'index spécifié. (3 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/commentcollection/add/#add_1)(string) | Ajoute un commentaire à la collection. |
| [Add](../../aspose.cells/commentcollection/add/#add)(int, int) | Ajoute un commentaire à la collection. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment/#addthreadedcomment_1)(string, string, ThreadedCommentAuthor) | Ajoute un commentaire en fil de discussion. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment/#addthreadedcomment)(int, int, string, ThreadedCommentAuthor) | Ajoute un commentaire en fil de discussion. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Comment) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Comment, IComparer&lt;Comment&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Comment, IComparer&lt;Comment&gt;) |  |
| [Clear](../../aspose.cells/commentcollection/clear/#clear)() | Supprime tous les commentaires ; (2 méthodes) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Comment) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Comment[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Comment[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Comment[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Comment&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Comment&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Comment&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Comment&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments/#getthreadedcomments_1)(string) | Obtient les commentaires en fil de discussion par nom de cellule. |
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments/#getthreadedcomments)(int, int) | Obtient les commentaires en fil de discussion par index de ligne et de colonne. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveAt](../../aspose.cells/commentcollection/removeat/#removeat_2)(string) | Supprime le commentaire de la cellule spécifique. |
| [RemoveAt](../../aspose.cells/commentcollection/removeat/#removeat_1)(int, int) | Supprime le commentaire de la cellule spécifique. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CommentCollectionDemo
    {
        public static void CommentCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à la collection de commentaires de la feuille de calcul
            CommentCollection comments = worksheet.Comments;

            // Ajouter un commentaire à la cellule A1
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Author = "Author1";
            comment1.Font.Name = "Times New Roman";

            // Ajoutez un commentaire à la cellule B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";
            comment2.Author = "Author2";

            // Ajouter un commentaire en fil de discussion à la cellule C3
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Author3", "user3", "provider3");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            comments.AddThreadedComment(2, 2, "This is a threaded comment.", author);

            // Récupérer les commentaires en fil de discussion de la cellule C3
            var threadedComments = comments.GetThreadedComments(2, 2);
            foreach (var threadedComment in threadedComments)
            {
                Console.WriteLine(threadedComment.Notes);
            }

            // Supprimer le commentaire à la cellule A1
            comments.RemoveAt(0, 0);

            // Effacer tous les commentaires
            comments.Clear();

            // Enregistrez le classeur
            workbook.Save("CommentCollectionExample.xlsx");
            workbook.Save("CommentCollectionExample.pdf");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Comment](../comment/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


