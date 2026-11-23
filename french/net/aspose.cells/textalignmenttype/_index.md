---
title: "Enum TextAlignmentType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.TextAlignmentType enum. Enumère les types d'alignement du texte"
type: docs
url: /fr/net/aspose.cells/textalignmenttype/
---
## TextAlignmentType enumeration

Énumère les types d'alignement du texte.

```csharp
public enum TextAlignmentType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| General | `1792` | Représente l'alignement de texte général. |
| Bottom | `528` | Représente l'alignement du texte en bas. |
| Center | `1802` | Représente l'alignement du texte centré. |
| CenterAcross | `1286` | Représente l'alignement du texte centré sur toute la largeur. |
| Distributed | `807` | Représente l'alignement du texte distribué. |
| Fill | `1284` | Représente l'alignement du texte remplissage. |
| Justify | `1821` | Représente l'alignement du texte justifié. |
| Left | `257` | Représente l'alignement du texte à gauche. |
| Right | `259` | Représente l'alignement du texte à droite. |
| Top | `512` | Représente l'alignement du texte en haut. |
| JustifiedLow | `832` | Aligne le texte avec une longueur de kashida ajustée pour le texte arabe. |
| ThaiDistributed | `896` | Distribue le texte thaï de manière spéciale, car chaque caractère est traité comme un mot. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TextAlignmentTypeDemo
    {
        public static void TextAlignmentTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(78);

            // Ajouter un commentaire à une cellule
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a comment.";
            comment.TextHorizontalAlignment = TextAlignmentType.Center;
            comment.TextVerticalAlignment = TextAlignmentType.Top;

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Personnaliser le titre du graphique
            chart.Title.Text = "Scores Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Enregistrez le classeur
            workbook.Save("TextAlignmentTypeExample.xlsx");

            // Afficher les résultats
            Console.WriteLine("Workbook saved successfully with text alignment settings.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


