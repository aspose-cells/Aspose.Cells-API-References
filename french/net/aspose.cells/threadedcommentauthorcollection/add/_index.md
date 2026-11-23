---
title: "ThreadedCommentAuthorCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ThreadedCommentAuthorCollection. Ajoute une personne de commentaire en fil"
type: docs
url: /fr/net/aspose.cells/threadedcommentauthorcollection/add/
---
## ThreadedCommentAuthorCollection.Add method

Ajoute une personne de commentaire en fil.

```csharp
public int Add(string name, string userId, string providerId)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la personne. |
| userId | String |  |
| providerId | String | L'identifiant du fournisseur |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un auteur de commentaire en fil
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Test Author", "testuser", "TA");

            // Obtenir l'auteur ajouté
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Ajouter des commentaires en fil en utilisant l'auteur
            worksheet.Comments.AddThreadedComment("C2", "First comment", author);
            worksheet.Comments.AddThreadedComment("C2", "Second comment", author);

            // Enregistrez le classeur
            workbook.Save("ThreadedCommentsExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


