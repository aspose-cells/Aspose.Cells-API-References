---
title: "ThreadedCommentCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadedCommentCollection. Obtient le commentaire en fil de discussion à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/threadedcommentcollection/item/
---
## ThreadedCommentCollection indexer

Obtient le commentaire en fil de discussion à l'index spécifié.

```csharp
public ThreadedComment this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'index |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "Initial comment";

            // Ajouter des commentaires en fil de discussion
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // Ajouter des auteurs
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Ajouter des commentaires en fil de discussion
            threadedComments.Add("Reply 1", authors[author1Index]);
            threadedComments.Add("Reply 2", authors[author2Index]);

            // Démontrer l'utilisation de la propriété Item
            ThreadedComment firstComment = threadedComments[0];
            ThreadedComment secondComment = threadedComments[1];

            Console.WriteLine("First comment author: " + firstComment.Author.Name);
            Console.WriteLine("Second comment author: " + secondComment.Author.Name);

            // Modifier l'auteur du deuxième commentaire
            secondComment.Author = authors[author1Index];
            Console.WriteLine("Updated second comment author: " + secondComment.Author.Name);

            // Enregistrez le classeur
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


