---
title: "Enum DataBarNegativeColorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.DataBarNegativeColorType enum. Spécifie si l’on doit utiliser la même couleur de bordure et de remplissage que les barres de données positives"
type: docs
url: /fr/net/aspose.cells/databarnegativecolortype/
---
## DataBarNegativeColorType enumeration

Spécifie s'il faut utiliser la même couleur de bordure et de remplissage que les barres de données positives.

```csharp
public enum DataBarNegativeColorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Color | `0` | Utilisez la couleur spécifiée dans la boîte de dialogue Valeur négative et réglage d'axe ou en utilisant les propriétés ColorType et BorderColorType de l'objet NegativeBarFormat. |
| SameAsPositive | `1` | Utilisez la même couleur que les barres de données positives. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarNegativeColorTypeDemo
    {
        public static void DataBarNegativeColorTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(-20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(-40);
            worksheet.Cells["A5"].PutValue(50);

            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Définir les propriétés de la barre de données
            DataBar dataBar = fc.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Number;
            dataBar.MinCfvo.Value = -50;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Number;
            dataBar.MaxCfvo.Value = 50;
            dataBar.Color = System.Drawing.Color.Green;

            // Définir les propriétés du format de la barre négative
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = System.Drawing.Color.Red;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = System.Drawing.Color.Blue;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.SameAsPositive;

            // Enregistrez le classeur
            workbook.Save("DataBarNegativeColorTypeExample.xlsx");
            workbook.Save("DataBarNegativeColorTypeExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


