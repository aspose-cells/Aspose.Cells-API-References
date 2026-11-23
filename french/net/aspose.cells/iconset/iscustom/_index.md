---
title: "IconSet.IsCustom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété IconSet. Indique si le jeu d'icônes est personnalisé. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/iconset/iscustom/
---
## IconSet.IsCustom property

Indique si le jeu d'icônes est personnalisé. La valeur par défaut est false.

```csharp
public bool IsCustom { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyIsCustomDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Ajouter une mise en forme conditionnelle avec un jeu d'icônes personnalisé
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Définir la plage pour la mise en forme conditionnelle
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 9;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Ajouter une condition d'ensemble d'icônes
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Définir le type du jeu d'icônes (en utilisant un IconSetType valide)
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Vérifier la propriété IsCustom (lecture seule)
            Console.WriteLine("Is IconSet custom? " + condition.IconSet.IsCustom);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


