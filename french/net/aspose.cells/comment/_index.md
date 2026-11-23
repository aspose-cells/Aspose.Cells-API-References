---
title: "Classe Comment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Comment. Encapsule l'objet qui représente un commentaire de cellule"
type: docs
url: /fr/net/aspose.cells/comment/
---
## Comment class

Encapsule l'objet qui représente un commentaire de cellule.

```csharp
public class Comment
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Author](../../aspose.cells/comment/author/) { get; set; } | Obtient et définit le nom de l'auteur original du commentaire |
| [AutoSize](../../aspose.cells/comment/autosize/) { get; set; } | Indique si la taille du commentaire est ajustée automatiquement en fonction de son contenu. Remarque : dans certains cas particuliers (comme l'environnement Mac), ce paramètre peut ne pas prendre effet. Si ce paramètre ne prend pas effet, veuillez le remplacer par FitToTextSize(). |
| [Column](../../aspose.cells/comment/column/) { get; } | Obtient l'index de colonne du commentaire. |
| [CommentShape](../../aspose.cells/comment/commentshape/) { get; } | Obtient un objet Shape qui représente la forme attachée au commentaire spécifié. |
| [Font](../../aspose.cells/comment/font/) { get; } | Obtient la police du commentaire. |
| [Height](../../aspose.cells/comment/height/) { get; set; } | Représente la hauteur du commentaire, en pixels. |
| [HeightCM](../../aspose.cells/comment/heightcm/) { get; set; } | Représente la hauteur du commentaire, en centimètres. |
| [HeightInch](../../aspose.cells/comment/heightinch/) { get; set; } | Représente la hauteur du commentaire, en pouces. |
| [HtmlNote](../../aspose.cells/comment/htmlnote/) { get; set; } | Obtient et définit la chaîne HTML qui contient les données et certains formats dans ce commentaire. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment/) { get; } | Indique si ce commentaire est un commentaire en fil de discussion. |
| [IsVisible](../../aspose.cells/comment/isvisible/) { get; set; } | Indique si le commentaire est visible ou non. |
| [Note](../../aspose.cells/comment/note/) { get; set; } | Représente le contenu du commentaire. |
| [Row](../../aspose.cells/comment/row/) { get; } | Obtient l'index de ligne du commentaire. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment/) { get; set; } | Obtient et définit le type d'alignement horizontal du texte du commentaire. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype/) { get; set; } | Obtient et définit le type d'orientation du texte du commentaire. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment/) { get; set; } | Obtient et définit le type d'alignement vertical du texte du commentaire. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments/) { get; } | Obtient la liste des commentaires en fil de discussion ; |
| [Width](../../aspose.cells/comment/width/) { get; set; } | Représente la largeur du commentaire, en pixels. |
| [WidthCM](../../aspose.cells/comment/widthcm/) { get; set; } | Représente la largeur du commentaire, en centimètres. |
| [WidthInch](../../aspose.cells/comment/widthinch/) { get; set; } | Représente la largeur du commentaire, en pouces. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters/)(int, int) | Renvoie un objet Characters qui représente une plage de caractères dans le texte du commentaire. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters/)(int, int, Font, StyleFlag) | Formate certains caractères avec le réglage de police. |
| [GetRichFormattings](../../aspose.cells/comment/getrichformattings/)() | Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte du commentaire. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CommentDemo
    {
        public static void CommentExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            // Accédez à la collection de commentaires de la feuille de calcul
            CommentCollection comments = worksheet.Comments;

            // Ajouter un commentaire à la cellule A1
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Font.Name = "Times New Roman";
            comment1.Font.Size = 12;
            comment1.Font.Color = System.Drawing.Color.Red;
            comment1.Author = "Carl.Yang";
            comment1.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            comment1.IsVisible = true;
            comment1.TextOrientationType = TextOrientationType.TopToBottom;
            comment1.TextHorizontalAlignment = TextAlignmentType.Center;
            comment1.TextVerticalAlignment = TextAlignmentType.Center;
            comment1.AutoSize = true;
            comment1.HeightCM = 1.0;
            comment1.WidthCM = 1.0;
            comment1.Width = 10;
            comment1.Height = 10;
            comment1.WidthInch = 1.0;
            comment1.HeightInch = 1.0;

            // Accédez à la forme du commentaire
            CommentShape shape = comment1.CommentShape;
            int w = shape.Width;
            int h = shape.Height;

            // Ajoutez un commentaire à la cellule B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";

            // Enregistrez le classeur
            workbook.Save("CommentExample.xlsx");
            workbook.Save("CommentExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


