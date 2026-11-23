---
title: "Enum DataBarAxisPosition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.DataBarAxisPosition enum. Spécifie la position de l'axe pour une plage de cellules avec un format conditionnel sous forme de barres de données"
type: docs
url: /fr/net/aspose.cells/databaraxisposition/
---
## DataBarAxisPosition enumeration

Spécifie la position de l'axe pour une plage de cellules avec mise en forme conditionnelle sous forme de barres de données.

```csharp
public enum DataBarAxisPosition
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Automatic | `0` | Affichez l'axe à une position variable en fonction du rapport entre la valeur négative minimale et la valeur positive maximale dans la plage. Les valeurs positives sont affichées dans une direction de gauche à droite. Les valeurs négatives sont affichées dans une direction de droite à gauche. Lorsque toutes les valeurs sont positives ou toutes les valeurs sont négatives, aucun axe n'est affiché. |
| Midpoint | `1` | Affichez l'axe au point médian de la cellule, quel que soit l'ensemble des valeurs dans la plage. Les valeurs positives sont affichées de gauche à droite. Les valeurs négatives sont affichées de droite à gauche. |
| None | `2` | Aucun axe n'est affiché, et les valeurs positives et négatives sont affichées dans la direction de gauche à droite. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarAxisPositionDemo
    {
        public static void DataBarAxisPositionExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            
            // Accès à la première feuille de calcul du classeur
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajout d'une règle de mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Définition de la plage de mise en forme conditionnelle
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);
            
            // Ajout d'une condition de barre de données
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];
            DataBar dataBar = fc.DataBar;
            
            // Définition des propriétés de la barre de données
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint; // Using DataBarAxisPosition enum
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
            
            // Insertion des valeurs de cellules
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);
            
            // Enregistrement du fichier Excel
            workbook.Save("DataBarAxisPositionExample.xlsx");
            workbook.Save("DataBarAxisPositionExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


