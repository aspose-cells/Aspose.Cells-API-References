---
title: "Classe NegativeBarFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.NegativeBarFormat. Représente les paramètres de couleur des barres de données pour les valeurs négatives qui sont définies par une règle de mise en forme conditionnelle de barre de données"
type: docs
url: /fr/net/aspose.cells/negativebarformat/
---
## NegativeBarFormat class

Représente les paramètres de couleur des barres de données pour les valeurs négatives définies par une règle de mise en forme conditionnelle de barre de données.

```csharp
public class NegativeBarFormat
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BorderColor](../../aspose.cells/negativebarformat/bordercolor/) { get; set; } | Obtient ou définit un objet FormatColor que vous pouvez utiliser pour spécifier la couleur de bordure des barres de données négatives. |
| [BorderColorType](../../aspose.cells/negativebarformat/bordercolortype/) { get; set; } | Indique s'il faut utiliser la même couleur de bordure que les barres de données positives. |
| [Color](../../aspose.cells/negativebarformat/color/) { get; set; } | Obtient ou définit un objet FormatColor que vous pouvez utiliser pour spécifier la couleur de remplissage des barres de données négatives. |
| [ColorType](../../aspose.cells/negativebarformat/colortype/) { get; set; } | Obtient ou définit s'il faut utiliser la même couleur de remplissage que les barres de données positives. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class NegativeBarFormatDemo
    {
        public static void NegativeBarFormatExample()
        {
            // Instanciez un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoute une mise en forme conditionnelle vide
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Définit la plage de mise en forme conditionnelle
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Ajoute une condition pour DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Obtenez DataBar et définissez ses propriétés
            DataBar dataBar = fc.DataBar;
            dataBar.Color = Color.Orange;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // Configurez les propriétés de NegativeBarFormat
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = Color.White;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = Color.Yellow;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;

            // Placez quelques valeurs dans les cellules
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);

            // Enregistrez le classeur
            workbook.Save("NegativeBarFormatExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


