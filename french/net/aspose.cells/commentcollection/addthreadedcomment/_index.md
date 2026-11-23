---
title: "CommentCollection.AddThreadedComment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CommentCollection. Ajoute un commentaire en fil"
type: docs
url: /fr/net/aspose.cells/commentcollection/addthreadedcomment/
---
## AddThreadedComment(int, int, string, ThreadedCommentAuthor) {#addthreadedcomment}

Ajoute un commentaire en fil de discussion.

```csharp
public int AddThreadedComment(int row, int column, string text, ThreadedCommentAuthor author)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne de Cell. |
| column | Int32 | Indice de colonne de Cell. |
| texte | String | Le texte du commentaire |
| auteur | ThreadedCommentAuthor | L'utilisateur de ce commentaire en fil. |

### Valeur de retour

[`ThreadedComment`](../../threadedcomment/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodAddThreadedCommentWithInt32Int32StringThreadedCommenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CommentCollection comments = worksheet.Comments;
            
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demoUser", "testProvider");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            
            comments.AddThreadedComment(1, 1, "This is a threaded comment demo.", author);
            
            var threadedComments = comments.GetThreadedComments(1, 1);
            foreach (var comment in threadedComments)
            {
                Console.WriteLine(comment.Notes);
            }

            workbook.Save("ThreadedCommentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddThreadedComment(string, string, ThreadedCommentAuthor) {#addthreadedcomment_1}

Ajoute un commentaire en fil de discussion.

```csharp
public int AddThreadedComment(string cellName, string text, ThreadedCommentAuthor author)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Le nom de la cellule. |
| texte | String | Le texte du commentaire |
| auteur | ThreadedCommentAuthor | L'utilisateur de ce commentaire en fil. |

### Valeur de retour

[`ThreadedComment`](../../threadedcomment/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodAddThreadedCommentWithStringStringThreadedCommentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            
            CommentCollection comments = worksheet.Comments;
            comments.AddThreadedComment("B3", "Initial comment text", author);
            comments.AddThreadedComment("C5", "Follow-up comment", author);
            
            workbook.Save("ThreadedCommentsOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


