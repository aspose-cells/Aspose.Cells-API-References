---
title: "Classe TableStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Tables.TableStyle. Représente le style du tableau"
type: docs
url: /fr/net/aspose.cells.tables/tablestyle/
---
## TableStyle class

Représente le style de la table.

```csharp
public class TableStyle
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Name](../../aspose.cells.tables/tablestyle/name/) { get; } | Obtient le nom du style de tableau. |
| [TableStyleElements](../../aspose.cells.tables/tablestyle/tablestyleelements/) { get; } | Obtient tous les éléments du style de tableau. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [Create](../../aspose.cells.tables/tablestyle/create/)(string, WorksheetCollection) | Crée un style de tableau/tableau croisé dynamique vide. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleDemo
    {
        public static void TableStyleExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créez des styles pour les première et dernière colonnes
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Définissez un nom de style de tableau personnalisé
            string tableStyleName = "Custom1";

            // Accédez à la collection des styles de tableau
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Ajoutez un nouveau style de tableau à la collection
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Accédez à la collection des éléments du style de tableau
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Ajoute et définit le style pour la première colonne
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Ajoute et définit le style pour la dernière colonne
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Accède aux cellules de la première feuille de calcul
            Cells cells = workbook.Worksheets[0].Cells;

            // Remplit la première ligne avec les noms de colonnes
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }

            // Remplit le reste des cellules avec des données d'exemple
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Ajoutez un tableau à la feuille de calcul
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Appliquez le style de tableau personnalisé au tableau
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Enregistrez le classeur
            workbook.Save("TableStyleExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


