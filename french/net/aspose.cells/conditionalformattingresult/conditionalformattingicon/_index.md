---
title: "ConditionalFormattingResult.ConditionalFormattingIcon"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConditionalFormattingResult. Obtient l'image du jeu d'icônes"
type: docs
url: /fr/net/aspose.cells/conditionalformattingresult/conditionalformattingicon/
---
## ConditionalFormattingResult.ConditionalFormattingIcon property

Obtient l'image du jeu d'icônes.

```csharp
public ConditionalFormattingIcon ConditionalFormattingIcon { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalFormattingIconDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple et un formatage conditionnel
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Ajouter une mise en forme conditionnelle d'ensemble d'icônes
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddArea(area);

            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Calculez les formules et obtenez le résultat du formatage conditionnel
            workbook.CalculateFormula();
            ConditionalFormattingResult result = worksheet.Cells["A1"].GetConditionalFormattingResult();

            // Démontrez la propriété ConditionalFormattingIcon
            if (result != null && result.ConditionalFormattingIcon != null)
            {
                Console.WriteLine("Icon Type: " + result.ConditionalFormattingIcon.Type);
                Console.WriteLine("Icon Index: " + result.ConditionalFormattingIcon.Index);
            }
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


