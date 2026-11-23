---
title: "Classe Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Row. Représente une ligne unique dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/row/
---
## Row class

Représente une seule ligne dans une feuille de calcul.

```csharp
public class Row : IEnumerable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [FirstCell](../../aspose.cells/row/firstcell/) { get; } | Obtient le premier objet cellule de la ligne. |
| [FirstDataCell](../../aspose.cells/row/firstdatacell/) { get; } | Obtient la première cellule non vide de la ligne. |
| [GroupLevel](../../aspose.cells/row/grouplevel/) { get; set; } | Obtient le niveau de groupe de la ligne. |
| [HasCustomStyle](../../aspose.cells/row/hascustomstyle/) { get; } | Indique si cette ligne possède des paramètres de style personnalisés(différents de ceux par défaut hérités du classeur). |
| [Height](../../aspose.cells/row/height/) { get; set; } | Obtient et définit la hauteur de la ligne en unités de points. |
| [Index](../../aspose.cells/row/index/) { get; } | Obtient l'index de cette ligne. |
| [IsBlank](../../aspose.cells/row/isblank/) { get; } | Indique si la ligne contient des données. |
| [IsCollapsed](../../aspose.cells/row/iscollapsed/) { get; set; } | si la ligne est réduite |
| [IsHeightMatched](../../aspose.cells/row/isheightmatched/) { get; set; } | Indique si la hauteur de la ligne correspond au paramètre de police par défaut actuel du classeur. La valeur true de cette propriété indique également que la hauteur de la ligne est "automatique" sans valeur de hauteur personnalisée définie par l'utilisateur. |
| [IsHidden](../../aspose.cells/row/ishidden/) { get; set; } | Indique si la ligne est masquée. |
| [Item](../../aspose.cells/row/item/) { get; } | Obtient la cellule. |
| [LastCell](../../aspose.cells/row/lastcell/) { get; } | Obtient le dernier objet cellule de la ligne. |
| [LastDataCell](../../aspose.cells/row/lastdatacell/) { get; } | Obtient la dernière cellule non vide de la ligne. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ApplyStyle](../../aspose.cells/row/applystyle/)(Style, StyleFlag) | Applique les formats à toute la ligne. |
| [CopySettings](../../aspose.cells/row/copysettings/)(Row, bool) | Copie les paramètres de la ligne, tels que le style, la hauteur, la visibilité, ...etc. |
| override [Equals](../../aspose.cells/row/equals/#equals_1)(object) | Vérifie si cet objet fait référence à la même ligne qu'un autre. |
| [Equals](../../aspose.cells/row/equals/#equals)(Row) | Vérifie si cet objet fait référence à la même ligne qu'un autre objet ligne. |
| [GetCellByIndex](../../aspose.cells/row/getcellbyindex/)(int) | Obtenez la cellule par un index spécifique dans la collection de cellules de cette ligne. |
| [GetCellOrNull](../../aspose.cells/row/getcellornull/)(int) | Obtient la cellule ou null à l'index spécifié. |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator)() | Obtient l'énumérateur des cellules |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator_1)(bool, bool) | Obtient un énumérateur qui parcourt les cellules de cette ligne. |
| [GetStyle](../../aspose.cells/row/getstyle/)() | Obtient le style de cette ligne. |
| [SetStyle](../../aspose.cells/row/setstyle/)(Style) | Définit le style de cette ligne. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;
    using System.Collections;

    public class RowDemo
    {
        public static void RowExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Obtention de la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez un objet de style
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

            // Obtenir la première ligne
            Row row = worksheet.Cells.Rows[0];

            // Appliquer le style à la première ligne
            row.ApplyStyle(style, styleFlag);

            // Définir les propriétés de la ligne
            row.Height = 20.0;
            row.IsHidden = false;
            row.IsCollapsed = false;
            row.GroupLevel = 1;
            row.IsHeightMatched = true;

            // Accéder aux cellules de la ligne
            Cell firstCell = row.FirstCell;
            Cell firstDataCell = row.FirstDataCell;
            Cell lastCell = row.LastCell;
            Cell lastDataCell = row.LastDataCell;

            // Vérifier si la ligne est vide
            bool isBlank = row.IsBlank;

            // Vérifier si la ligne a un style personnalisé
            bool hasCustomStyle = row.HasCustomStyle;

            // Obtenir l'index de la ligne
            int rowIndex = row.Index;

            // Obtenir une cellule par index
            Cell cellByIndex = row.GetCellByIndex(0);

            // Obtenir le style de la ligne
            Style rowStyle = row.GetStyle();

            // Définir le style de la ligne
            row.SetStyle(rowStyle);

            // Copier les paramètres d'une autre ligne
            Row sourceRow = worksheet.Cells.Rows[1];
            row.CopySettings(sourceRow, true);

            // Énumérer les cellules de la ligne
            IEnumerator cellEnumerator = row.GetEnumerator();
            while (cellEnumerator.MoveNext())
            {
                Cell cell = (Cell)cellEnumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Enregistrement du fichier Excel
            workbook.Save("RowExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


