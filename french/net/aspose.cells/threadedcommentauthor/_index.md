---
title: "Classe ThreadedCommentAuthor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ThreadedCommentAuthor. Représente la personne qui crée les commentaires en fil"
type: docs
url: /fr/net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

Représente la personne qui crée les commentaires en fil de discussion.

```csharp
public class ThreadedCommentAuthor
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Name](../../aspose.cells/threadedcommentauthor/name/) { get; set; } | Obtient et définit le nom. |
| [ProviderId](../../aspose.cells/threadedcommentauthor/providerid/) { get; set; } | Obtient l'identifiant du fournisseur. |
| [UserId](../../aspose.cells/threadedcommentauthor/userid/) { get; set; } | Obtient et définit l'identifiant de l'utilisateur. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire
            int commentIndex = worksheet.Comments.Add("C1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            
            // Ajouter des auteurs de commentaires en fil
            int authorIndex1 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author1", "user1", "");
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex1];
            
            // Ajouter un commentaire en fil
            int threadedCommentIndex = comment.ThreadedComments.Add("Threaded comment text", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Accéder et modifier l'auteur
            Console.WriteLine("Original author: " + threadedComment.Author.Name);
            threadedComment.Author.Name = "ModifiedAuthor";
            Console.WriteLine("Modified author: " + threadedComment.Author.Name);

            // Créer un nouvel auteur et l'assigner
            int authorIndex2 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author2", "user2", "");
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex2];
            threadedComment.Author = author2;
            Console.WriteLine("New author: " + threadedComment.Author.Name);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


