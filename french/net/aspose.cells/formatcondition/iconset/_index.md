---
title: "FormatCondition.IconSet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "FormatCondition propriété. Obtenir l'instance IconSet du formatage conditionnel. Le type d'instance par défaut IconSetType est TrafficLights31. Valide uniquement pour le type IconSet"
type: docs
url: /fr/net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

Obtenez l'instance "IconSet" de la mise en forme conditionnelle. Le type IconSetType de l'instance par défaut est TrafficLights31. Valide uniquement pour le type = IconSet.

```csharp
public IconSet IconSet { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyIconSetDemo
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

            // Ajouter une mise en forme conditionnelle
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Définir la plage de cellules
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Ajouter une condition et définir le type sur IconSet
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Obtenir l'IconSet et le configurer
            IconSet iconSet = condition.IconSet;
            iconSet.Type = IconSetType.TrafficLights31;
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Enregistrez le classeur
            workbook.Save("IconSetDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


