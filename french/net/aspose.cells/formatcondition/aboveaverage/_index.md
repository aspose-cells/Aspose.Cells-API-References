---
title: "FormatCondition.AboveAverage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. Obtient l'instance AboveAverage du formatage conditionnel. La règle d'instance par défaut met en surbrillance les cellules dont la valeur est supérieure à la moyenne pour toutes les valeurs de la plage. Valide uniquement pour le type AboveAverage"
type: docs
url: /fr/net/aspose.cells/formatcondition/aboveaverage/
---
## FormatCondition.AboveAverage property

Obtenez l'instance "AboveAverage" de la mise en forme conditionnelle. La règle de l'instance par défaut met en surbrillance les cellules dont la valeur est supérieure à la moyenne de toutes les valeurs de la plage. Valide uniquement pour le type = AboveAverage.

```csharp
public AboveAverage AboveAverage { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyAboveAverageDemo
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

            // Ajouter un formatage conditionnel au-dessus de la moyenne
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 4, EndColumn = 0 });

            // Définir pour mettre en surbrillance les valeurs supérieures à la moyenne
            FormatCondition fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = true;
            fc.Style.BackgroundColor = Color.Yellow;

            // Ajouter un formatage conditionnel en dessous de la moyenne
            index = worksheet.ConditionalFormattings.Add();
            fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 1, EndRow = 4, EndColumn = 1 });

            // Définir pour mettre en surbrillance les valeurs inférieures à la moyenne
            fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = false;
            fc.Style.BackgroundColor = Color.LightBlue;

            // Enregistrez le classeur
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AboveAverage](../../aboveaverage/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


