---
title: "FormatCondition.DataBar"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. Obtient l'instance DataBar du formatage conditionnel. La couleur d'instance par défaut est bleue. Valide uniquement pour le type DataBar"
type: docs
url: /fr/net/aspose.cells/formatcondition/databar/
---
## FormatCondition.DataBar property

Obtenez l'instance "DataBar" de la mise en forme conditionnelle. La couleur de l'instance par défaut est bleue. Valide uniquement pour le type = DataBar.

```csharp
public DataBar DataBar { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyDataBarDemo
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

            // Ajouter une mise en forme conditionnelle de barre de données
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Définir la plage pour le formatage conditionnel
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Ajouter une condition de barre de données et définir les propriétés
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcs[conditionIndex];
            
            // Configurer les propriétés DataBar
            DataBar dataBar = condition.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            dataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            dataBar.Color = System.Drawing.Color.Green;

            // Enregistrez le classeur
            workbook.Save("DataBarExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


