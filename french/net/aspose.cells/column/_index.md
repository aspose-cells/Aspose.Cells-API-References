---
title: "Classe Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Column class. Représente une seule colonne dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/column/
---
## Column class

Représente une colonne unique dans une feuille de calcul.

```csharp
public class Column
```

## Propriétés

| Nom | Description |
| --- | --- |
| [GroupLevel](../../aspose.cells/column/grouplevel/) { get; set; } | Obtient le niveau de groupe de la colonne. |
| [HasCustomStyle](../../aspose.cells/column/hascustomstyle/) { get; } | Indique si cette colonne possède des paramètres de style personnalisés (différents du paramètre par défaut hérité du classeur). |
| [Index](../../aspose.cells/column/index/) { get; } | Obtient l'index de cette colonne. |
| [IsCollapsed](../../aspose.cells/column/iscollapsed/) { get; set; } | si la colonne est réduite |
| [IsHidden](../../aspose.cells/column/ishidden/) { get; set; } | Indique si la colonne est masquée. |
| [Style](../../aspose.cells/column/style/) { get; } | (**Obsolete.**) Obtient le style de cette colonne. |
| [Width](../../aspose.cells/column/width/) { get; set; } | Obtient et définit la largeur de la colonne en unités de caractères. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ApplyStyle](../../aspose.cells/column/applystyle/)(Style, StyleFlag) | Applique des formats à une colonne entière. |
| [GetStyle](../../aspose.cells/column/getstyle/)() | Obtient le style de cette colonne. |
| [SetStyle](../../aspose.cells/column/setstyle/)(Style) | Définit le style de cette colonne. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnDemo
    {
        public static void ColumnExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Obtention de la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un nouveau Style au classeur
            Style style = workbook.CreateStyle();

            // Définition de la couleur d'arrière-plan en bleu
            style.BackgroundColor = Color.Blue;

            // Définition de la couleur de premier plan en rouge
            style.ForegroundColor = Color.Red;

            // Définition du motif d'arrière-plan
            style.Pattern = BackgroundType.DiagonalStripe;

            // Nouveau drapeau de style
            StyleFlag styleFlag = new StyleFlag();

            // Définir tous les styles
            styleFlag.All = true;

            // Obtenir la première colonne
            Column column = worksheet.Cells.Columns[0];

            // Appliquer le style à la première colonne
            column.ApplyStyle(style, styleFlag);

            // Définition de propriétés supplémentaires
            column.Width = 20.0; // Setting the column width
            column.IsHidden = false; // Setting the column visibility
            column.IsCollapsed = false; // Setting the column collapsed state

            // Enregistrement du fichier Excel
            workbook.Save("ColumnExample.xlsx");
            workbook.Save("ColumnExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


