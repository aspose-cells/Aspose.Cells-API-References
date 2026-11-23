---
title: "Enum TextOrientationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.TextOrientationType enum. Énumère les types d'orientation du texte"
type: docs
url: /fr/net/aspose.cells/textorientationtype/
---
## TextOrientationType enumeration

Énumère les types d'orientation du texte.

```csharp
public enum TextOrientationType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| ClockWise | `0` | Fait pivoter le texte de 90 degrés dans le sens horaire. |
| CounterClockWise | `1` | Fait pivoter le texte de 90 degrés dans le sens antihoraire. |
| NoRotation | `2` | Représente la valeur par défaut. |
| TopToBottom | `3` | Affiche le texte de haut en bas de la cellule. Texte empilé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextOrientationTypeDemo
    {
        public static void TextOrientationTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");
            worksheet.Cells["A2"].PutValue("This is a test comment.");

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add(0, 0);
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment with text orientation.";

            // Définir différents types d'orientation du texte pour le commentaire
            comment.TextOrientationType = TextOrientationType.ClockWise;
            Console.WriteLine("Text Orientation: ClockWise");

            // Enregistrez le classeur
            workbook.Save("TextOrientationTypeExample_ClockWise.xlsx");

            // Changer l'orientation du texte en CounterClockWise
            comment.TextOrientationType = TextOrientationType.CounterClockWise;
            Console.WriteLine("Text Orientation: CounterClockWise");

            // Enregistrez le classeur
            workbook.Save("TextOrientationTypeExample_CounterClockWise.xlsx");

            // Changer l'orientation du texte en NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Text Orientation: NoRotation");

            // Enregistrez le classeur
            workbook.Save("TextOrientationTypeExample_NoRotation.xlsx");

            // Changer l'orientation du texte en TopToBottom
            comment.TextOrientationType = TextOrientationType.TopToBottom;
            Console.WriteLine("Text Orientation: TopToBottom");

            // Enregistrez le classeur
            workbook.Save("TextOrientationTypeExample_TopToBottom.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


