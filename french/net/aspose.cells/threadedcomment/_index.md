---
title: "Classe ThreadedComment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ThreadedComment. Représente le commentaire en fil de discussion"
type: docs
url: /fr/net/aspose.cells/threadedcomment/
---
## ThreadedComment class

Représente le commentaire en fil de discussion.

```csharp
public class ThreadedComment
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Author](../../aspose.cells/threadedcomment/author/) { get; set; } | Obtient l'auteur du commentaire. |
| [Column](../../aspose.cells/threadedcomment/column/) { get; } | Obtient l'index de colonne du commentaire. |
| [CreatedTime](../../aspose.cells/threadedcomment/createdtime/) { get; set; } | Obtient et définit l'heure de création de ce commentaire en fil de discussion. |
| [Notes](../../aspose.cells/threadedcomment/notes/) { get; set; } | Obtient et définit le texte du commentaire. |
| [Row](../../aspose.cells/threadedcomment/row/) { get; } | Obtient l'index de ligne du commentaire. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des auteurs au classeur
            int author1Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User1", "user1@example.com", "1");
            int author2Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User2", "", "2");
            
            // Obtenir les références d'auteur
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[author1Id];
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[author2Id];
            
            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Ajouter un commentaire en fil de discussion au commentaire
            int threadedCommentIndex = comment.ThreadedComments.Add("This is a threaded comment", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Définir des propriétés supplémentaires
            threadedComment.Notes = "Additional notes";
            
            // Ajouter une réponse au commentaire en fil de discussion
            int replyIndex = comment.ThreadedComments.Add("This is a reply", author2);
            ThreadedComment reply = comment.ThreadedComments[replyIndex];
            
            // Enregistrez le classeur
            workbook.Save("ThreadedCommentDemo.xlsx");
            
            Console.WriteLine("Threaded comment demo completed.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


