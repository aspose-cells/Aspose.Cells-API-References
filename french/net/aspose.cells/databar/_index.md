---
title: "Class DataBar"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DataBar. Décrit la règle de mise en forme conditionnelle DataBar. Cette règle de mise en forme conditionnelle affiche une barre de données graduée dans la plage de cellules"
type: docs
url: /fr/net/aspose.cells/databar/
---
## DataBar class

Décrit la règle de mise en forme conditionnelle DataBar. Cette règle de mise en forme conditionnelle affiche une dataBar graduée dans la plage de cellules.

```csharp
public class DataBar
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor/) { get; set; } | Obtient la couleur de l'axe pour les cellules avec une mise en forme conditionnelle sous forme de barres de données. |
| [AxisPosition](../../aspose.cells/databar/axisposition/) { get; set; } | Obtient ou définit la position de l'axe des barres de données spécifié par une règle de mise en forme conditionnelle. |
| [BarBorder](../../aspose.cells/databar/barborder/) { get; } | Obtient un objet qui spécifie la bordure d'une barre de données. |
| [BarFillType](../../aspose.cells/databar/barfilltype/) { get; set; } | Obtient ou définit comment une barre de données est remplie de couleur. |
| [Color](../../aspose.cells/databar/color/) { get; set; } | Obtenir ou définir la couleur de ce DataBar. |
| [Direction](../../aspose.cells/databar/direction/) { get; set; } | Obtient ou définit la direction dans laquelle le DataBar est affiché. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo/) { get; } | Obtenir ou définir l'objet de valeur maximale de ce DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Min. |
| [MaxLength](../../aspose.cells/databar/maxlength/) { get; set; } | Représente la longueur maximale du DataBar. |
| [MinCfvo](../../aspose.cells/databar/mincfvo/) { get; } | Obtenir ou définir l'objet de valeur minimale de ce DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max. |
| [MinLength](../../aspose.cells/databar/minlength/) { get; set; } | Représente la longueur minimale du DataBar. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat/) { get; } | Obtient l'objet NegativeBarFormat associé à une règle de mise en forme conditionnelle de DataBar. |
| [ShowValue](../../aspose.cells/databar/showvalue/) { get; set; } | Obtenir ou définir le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles ce DataBar est appliqué. La valeur par défaut est true. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage/)(Cell, ImageOrPrintOptions) | Rendre le DataBar dans la cellule en tableau d'octets d'image. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarDemo
    {
        public static void DataBarExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoute une mise en forme conditionnelle vide
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Définit la plage de mise en forme conditionnelle
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Ajoute une condition
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Obtenir DataBar
            DataBar dataBar = cond.DataBar;

            // Définir les propriétés du DataBar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Définir les valeurs des cellules
            Aspose.Cells.Cell cell1 = sheet.Cells["A1"];
            cell1.PutValue(10);
            Aspose.Cells.Cell cell2 = sheet.Cells["A2"];
            cell2.PutValue(120);
            Aspose.Cells.Cell cell3 = sheet.Cells["A3"];
            cell3.PutValue(260);

            // Enregistrement du fichier Excel
            workbook.Save("DataBarExample.xlsx");
            workbook.Save("DataBarExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


