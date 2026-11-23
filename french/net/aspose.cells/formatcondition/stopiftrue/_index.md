---
title: "FormatCondition.StopIfTrue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. True aucune règle avec une priorité inférieure ne peut être appliquée à cette règle lorsque celle‑ci s'évalue à true. S'applique uniquement à Excel 2007"
type: docs
url: /fr/net/aspose.cells/formatcondition/stopiftrue/
---
## FormatCondition.StopIfTrue property

Vrai, aucune règle avec une priorité inférieure ne peut être appliquée au-dessus de cette règle, lorsque celle‑ci s'évalue à vrai. S'applique uniquement à Excel 2007 ;

```csharp
public bool StopIfTrue { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStopIfTrueDemo
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

            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Ajouter une condition et définir StopIfTrue
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            FormatCondition condition = fcs[conditionIndex];
            condition.StopIfTrue = true;
            
            // Ajouter une autre condition qui remplacerait normalement la première
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "25", "");
            FormatCondition condition2 = fcs[conditionIndex2];
            condition2.StopIfTrue = false;

            // Enregistrez le classeur
            workbook.Save("StopIfTrueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


