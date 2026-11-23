---
title: "WorksheetCollection.ThreadedCommentAuthors"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WorksheetCollection propriété. Obtient la liste des auteurs de commentaires en fil"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/threadedcommentauthors/
---
## WorksheetCollection.ThreadedCommentAuthors property

Obtient la liste des auteurs de commentaires en fil.

```csharp
public ThreadedCommentAuthorCollection ThreadedCommentAuthors { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyThreadedCommentAuthorsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un auteur de commentaire en fil
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demo", "DA");

            // Obtenir l'auteur que nous venons d'ajouter
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Ajouter des commentaires en fil à la cellule C2
            AddThreadedComment(worksheet, "C2", "First comment", author);
            AddThreadedComment(worksheet, "C2", "Second comment", author);
            AddThreadedComment(worksheet, "C2", "Third comment", author);

            // Enregistrez le classeur
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }

        private static void AddThreadedComment(Worksheet worksheet, string cellName, string text, ThreadedCommentAuthor author)
        {
            // Obtenir la cellule où nous voulons ajouter le commentaire
            Cell cell = worksheet.Cells[cellName];
            
            // Ajouter un commentaire en fil (renvoie void, pas ThreadedComment)
            worksheet.Comments.AddThreadedComment(cellName, text, author);
        }
    }
}
```

### Voir aussi

* class [ThreadedCommentAuthorCollection](../../threadedcommentauthorcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


