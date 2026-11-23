---
title: "ColorScale.MidCfvo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ColorScale. Obtient ou définit cet objet de valeur moyenne de ColorScale. Impossible de définir CFValueObject avec le type FormatConditionValueType.Max ou FormatConditionValueType.Min."
type: docs
url: /fr/net/aspose.cells/colorscale/midcfvo/
---
## ColorScale.MidCfvo property

Obtenir ou définir l'objet de valeur intermédiaire de ce ColorScale. Impossible de définir CFValueObject avec le type FormatConditionValueType.Max ou FormatConditionValueType.Min.

```csharp
public ConditionalFormattingValue MidCfvo { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMidCfvoDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Ajouter une mise en forme conditionnelle d'échelle de couleur
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            int conditionIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            
            // Définir la valeur du point médian pour l'échelle de couleur
            ColorScale colorScale = fcc[conditionIndex].ColorScale;
            colorScale.MidCfvo.Type = FormatConditionValueType.Number;
            colorScale.MidCfvo.Value = 50;

            // Enregistrez le classeur
            workbook.Save("ColorScalePropertyMidCfvoDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


