---
title: "FormatCondition.ColorScale"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. Obtient l'instance ColorScale du formatage conditionnel. L'instance par défaut est un 3ColorScale vert-jaune-rouge. Valide uniquement pour le type ColorScale"
type: docs
url: /fr/net/aspose.cells/formatcondition/colorscale/
---
## FormatCondition.ColorScale property

Obtenez l'instance "ColorScale" de la mise en forme conditionnelle. L'instance par défaut est une échelle de couleurs "vert-jaune-rouge" 3ColorScale. Valide uniquement pour le type = ColorScale.

```csharp
public ColorScale ColorScale { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyColorScaleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Ajouter une mise en forme conditionnelle d'échelle de couleur
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Définir la plage pour la mise en forme conditionnelle
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Définir les propriétés de l'échelle de couleurs
            fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[0];
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Green;

            // Enregistrez le classeur
            workbook.Save("ColorScaleExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [ColorScale](../../colorscale/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


