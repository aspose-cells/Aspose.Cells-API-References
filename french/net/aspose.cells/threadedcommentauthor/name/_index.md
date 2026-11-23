---
title: "ThreadedCommentAuthor.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadedCommentAuthor. Obtient et définit le nom"
type: docs
url: /fr/net/aspose.cells/threadedcommentauthor/name/
---
## ThreadedCommentAuthor.Name property

Obtient et définit le nom.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire et des commentaires en fil
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            
            // Ajouter des commentaires en fil avec différents auteurs
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Ajouter des commentaires en fil de discussion
            threadedComments.Add("Reply from User1", authors[author1Index]);
            threadedComments.Add("Reply from User2", authors[author2Index]);

            // Démontrer l'utilisation de la propriété Name
            Console.WriteLine("First author name: " + threadedComments[0].Author.Name);
            Console.WriteLine("Second author name: " + threadedComments[1].Author.Name);

            // Modifier l'auteur du deuxième commentaire
            threadedComments[1].Author = authors[author1Index];
            Console.WriteLine("Updated second author name: " + threadedComments[1].Author.Name);

            // Enregistrez le classeur
            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


