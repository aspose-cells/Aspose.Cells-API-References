---
title: "Classe ColorScale"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ColorScale. Décrit la règle de mise en forme conditionnelle ColorScale. Cette règle de mise en forme conditionnelle crée une échelle de couleur graduée sur les cellules"
type: docs
url: /fr/net/aspose.cells/colorscale/
---
## ColorScale class

Décrit la règle de mise en forme conditionnelle ColorScale. Cette règle de mise en forme conditionnelle crée une échelle de couleur graduée sur les cellules.

```csharp
public class ColorScale
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Is3ColorScale](../../aspose.cells/colorscale/is3colorscale/) { get; set; } | Indique si la mise en forme conditionnelle est une échelle de couleur à 3 tons. |
| [MaxCfvo](../../aspose.cells/colorscale/maxcfvo/) { get; } | Obtenir ou définir l'objet de valeur maximale de ce ColorScale. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Min. |
| [MaxColor](../../aspose.cells/colorscale/maxcolor/) { get; set; } | Obtenir ou définir la couleur du dégradé pour la valeur maximale dans la plage. |
| [MidCfvo](../../aspose.cells/colorscale/midcfvo/) { get; } | Obtenir ou définir l'objet de valeur intermédiaire de ce ColorScale. Impossible de définir CFValueObject avec le type FormatConditionValueType.Max ou FormatConditionValueType.Min. |
| [MidColor](../../aspose.cells/colorscale/midcolor/) { get; set; } | Obtenir ou définir la couleur du dégradé pour la valeur médiane dans la plage. |
| [MinCfvo](../../aspose.cells/colorscale/mincfvo/) { get; } | Obtenir ou définir l'objet de valeur minimale de ce ColorScale. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max. |
| [MinColor](../../aspose.cells/colorscale/mincolor/) { get; set; } | Obtenir ou définir la couleur du dégradé pour la valeur minimale dans la plage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColorScaleDemo
    {
        public static void ColorScaleExample()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Ajouter une règle de mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 9 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Accéder à l'objet ColorScale
            ColorScale colorScale = fc.ColorScale;

            // Définir les propriétés du ColorScale
            colorScale.Is3ColorScale = true;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Définir les objets de valeur min, méd et max
            ConditionalFormattingValue minCfvo = colorScale.MinCfvo;
            minCfvo.Type = FormatConditionValueType.Min;
            minCfvo.Value = null;

            ConditionalFormattingValue midCfvo = colorScale.MidCfvo;
            midCfvo.Type = FormatConditionValueType.Percentile;
            midCfvo.Value = 50;

            ConditionalFormattingValue maxCfvo = colorScale.MaxCfvo;
            maxCfvo.Type = FormatConditionValueType.Max;
            maxCfvo.Value = null;

            // Enregistrez le classeur
            workbook.Save("ColorScaleExample.xlsx");
            workbook.Save("ColorScaleExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


