---
title: "ColorScale.MinCfvo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ColorScale. Obtient ou définit cet objet de valeur minimale de ColorScale. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max."
type: docs
url: /fr/net/aspose.cells/colorscale/mincfvo/
---
## ColorScale.MinCfvo property

Obtenir ou définir l'objet de valeur minimale de ce ColorScale. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinCfvoDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Créer une mise en forme conditionnelle d'échelle de couleur
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Ajouter une échelle de couleur
            int csIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            ColorScale cs = fcc[csIndex].ColorScale;

            // Définir les propriétés MinCfvo
            cs.MinCfvo.Type = FormatConditionValueType.Min;
            cs.MinCfvo.Value = "0";
            cs.MinColor = System.Drawing.Color.Red;

            // Définir les propriétés MidCfvo
            cs.MidCfvo.Type = FormatConditionValueType.Percentile;
            cs.MidCfvo.Value = "50";
            cs.MidColor = System.Drawing.Color.Yellow;

            // Définir les propriétés MaxCfvo
            cs.MaxCfvo.Type = FormatConditionValueType.Max;
            cs.MaxCfvo.Value = "0";
            cs.MaxColor = System.Drawing.Color.Green;

            // Enregistrez le classeur
            workbook.Save("ColorScaleMinCfvoDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


