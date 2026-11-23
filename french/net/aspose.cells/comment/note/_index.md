---
title: "Comment.Note"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Représente le contenu du commentaire"
type: docs
url: /fr/net/aspose.cells/comment/note/
---
## Comment.Note property

Représente le contenu du commentaire.

```csharp
public string Note { get; set; }
```

### Remarques

Si c'est un commentaire en fil, la note ne peut pas être modifiée, sinon MS Excel ne pourrait pas le traiter comme un commentaire en fil.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyNoteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            
            // Définir la note du commentaire
            comment1.Note = "First note.";
            
            // Vérifier que la note a été définie
            Console.WriteLine("Comment note: " + comment1.Note);
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


