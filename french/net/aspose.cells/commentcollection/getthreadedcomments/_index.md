---
title: "CommentCollection.GetThreadedComments"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CommentCollection. Obtient les commentaires en fil de discussion par indice de ligne et de colonne"
type: docs
url: /fr/net/aspose.cells/commentcollection/getthreadedcomments/
---
## GetThreadedComments(int, int) {#getthreadedcomments}

Obtient les commentaires en fil de discussion par index de ligne et de colonne.

```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |

### Exemples

```csharp

[C#]
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.Count; ++i)
{
    ThreadedComment tc = threadedComments1[i];
    string note = tc.Notes;
}
```

### Voir aussi

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetThreadedComments(string) {#getthreadedcomments_1}

Obtient les commentaires en fil de discussion par nom de cellule.

```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Le nom de la cellule. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodGetThreadedCommentsWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un auteur de commentaire en fil de discussion et récupérez l'auteur par indice
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "1");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Ajoutez un commentaire en fil de discussion à la cell B2
            worksheet.Comments.AddThreadedComment("B2", "Initial comment", author);

            // Obtenir tous les commentaires en fil pour la cellule B2
            ThreadedCommentCollection threadedComments = worksheet.Comments.GetThreadedComments("B2");

            // Afficher les commentaires en fil
            foreach (ThreadedComment comment in threadedComments)
            {
                Console.WriteLine($"Comment by {comment.Author.Name}: {comment.Notes}");
            }
        }
    }
}
```

### Voir aussi

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


