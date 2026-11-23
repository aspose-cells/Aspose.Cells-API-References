---
title: "Énum TableStyleElementType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Tables.TableStyleElementType enum. Représente le type d'élément de style du tableau ou du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.tables/tablestyleelementtype/
---
## TableStyleElementType enumeration

Représente le type d'élément de style de Table ou de Tableau croisé dynamique.

```csharp
public enum TableStyleElementType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| BlankRow | `18` | Élément de style de tableau qui s'applique aux lignes vides du tableau croisé dynamique. |
| FirstColumn | `8` | Élément de style de tableau qui s'applique à la première colonne du tableau. |
| FirstColumnStripe | `3` | Élément de style de tableau qui s'applique aux bandes de la première colonne du tableau. |
| FirstColumnSubheading | `22` | Élément de style de tableau qui s'applique au sous-titre de la première colonne du tableau croisé dynamique. |
| FirstHeaderCell | `11` | Élément de style de tableau qui s'applique à la première cellule de la ligne d'en-tête du tableau. |
| FirstRowStripe | `5` | Élément de style de tableau qui s'applique aux bandes de la première ligne du tableau. |
| FirstRowSubheading | `25` | Élément de style de tableau qui s'applique au sous-titre de la première ligne du tableau croisé dynamique. |
| FirstSubtotalColumn | `15` | Élément de style de tableau qui s'applique à la première colonne de sous-total du tableau croisé dynamique. |
| FirstSubtotalRow | `19` | Élément de style de tableau qui s'applique à la première ligne de sous-total du tableau croisé dynamique. |
| GrandTotalColumn | `28` | Élément de style de tableau qui s'applique à la colonne du total général du tableau croisé dynamique. |
| GrandTotalRow | `29` | Élément de style de tableau qui s'applique à la ligne du total général du tableau croisé dynamique. |
| FirstTotalCell | `13` | Élément de style de tableau qui s'applique à la première cellule de la ligne de total du tableau. |
| HeaderRow | `9` | Élément de style de tableau qui s'applique à la ligne d'en-tête du tableau. |
| LastColumn | `7` | Élément de style de tableau qui s'applique à la dernière colonne du tableau. |
| LastHeaderCell | `12` | Élément de style de tableau qui s'applique à la dernière cellule de la ligne d'en-tête du tableau. |
| LastTotalCell | `14` | Élément de style de tableau qui s'applique à la dernière cellule de la ligne de total du tableau. |
| PageFieldLabels | `1` | Élément de style de tableau qui s'applique aux libellés de champ de page du tableau croisé dynamique. |
| PageFieldValues | `2` | Élément de style de tableau qui s'applique aux valeurs du champ de page de la table pivot. |
| SecondColumnStripe | `4` | Élément de style de tableau qui s'applique aux bandes de la deuxième colonne de la Table. |
| SecondColumnSubheading | `23` | Élément de style de tableau qui s'applique au sous-titre de la deuxième colonne de la table pivot. |
| SecondRowStripe | `6` | Élément de style de tableau qui s'applique aux bandes de la deuxième ligne de la Table. |
| SecondRowSubheading | `26` | Élément de style de tableau qui s'applique au sous-titre de la deuxième ligne de la table pivot. |
| SecondSubtotalColumn | `16` | Élément de style de tableau qui s'applique à la deuxième colonne de sous-total de la PivotTable. |
| SecondSubtotalRow | `20` | Élément de style de tableau qui s'applique à la deuxième ligne de sous-total de la PivotTable. |
| ThirdColumnSubheading | `24` | Élément de style de tableau qui s'applique au sous-titre de la troisième colonne de la PivotTable. |
| ThirdRowSubheading | `27` | Élément de style de tableau qui s'applique au sous-titre de la troisième ligne de la PivotTable. |
| ThirdSubtotalColumn | `17` | Élément de style de tableau qui s'applique à la troisième colonne de sous-total de la table pivot. |
| ThirdSubtotalRow | `21` | Élément de style de tableau qui s'applique à la troisième ligne de sous-total de la PivotTable. |
| TotalRow | `10` | Élément de style de tableau qui s'applique à la ligne totale de la Table. |
| WholeTable | `0` | Élément de style de tableau qui s'applique à l'intégralité du contenu de la Table. |
| LastColumnSubheading | `130` | Élément de style de tableau qui s'applique au champ de la dernière colonne de la table pivot. |
| LastRowSubheading | `131` | Élément de style de tableau qui s'applique au champ de la dernière ligne de la table pivot. |
| LastSubtotalRow | `133` | Élément de style de tableau qui s'applique au champ de la dernière ligne de sous-total de la table pivot. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TablesClassTableStyleElementTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            
            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.ForegroundColor = System.Drawing.Color.LightGreen;

            string tableStyleName = "CustomStyle1";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            elements[elementIndex].SetElementStyle(firstColumnStyle);
            
            elementIndex = elements.Add(TableStyleElementType.LastColumn);
            elements[elementIndex].SetElementStyle(lastColumnStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue($"Column {i + 1}");
            }

            for (int row = 1; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue(row * col);
                }
            }

            ListObject table = workbook.Worksheets[0].ListObjects[workbook.Worksheets[0].ListObjects.Add(0, 0, 4, 4, true)];
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


