---
title: "FormatCondition.Priority"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. La priorité de cette règle de mise en forme conditionnelle. Cette valeur est utilisée pour déterminer quel format doit être évalué et rendu. Les valeurs numériques plus faibles ont une priorité plus élevée que les valeurs numériques plus élevées, où 1 est la priorité la plus haute."
type: docs
url: /fr/net/aspose.cells/formatcondition/priority/
---
## FormatCondition.Priority property

La priorité de cette règle de mise en forme conditionnelle. Cette valeur est utilisée pour déterminer quel format doit être évalué et rendu. Les valeurs numériques plus faibles ont une priorité plus élevée que les valeurs numériques plus élevées, où '1' représente la priorité la plus haute.

```csharp
public int Priority { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyPriorityDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Ajouter une mise en forme conditionnelle
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            
            // Ajouter des conditions
            int conditionIndex1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "2", "5");
            int conditionIndex2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "6", "9");

            // Définir les priorités
            formatConditions[conditionIndex1].Priority = 2;
            formatConditions[conditionIndex2].Priority = 1;

            // Démontrer l'utilisation de la propriété Priority
            Console.WriteLine("Condition 1 Priority: " + formatConditions[conditionIndex1].Priority);
            Console.WriteLine("Condition 2 Priority: " + formatConditions[conditionIndex2].Priority);

            // Enregistrez le classeur
            workbook.Save("ConditionalFormattingPriorityDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


