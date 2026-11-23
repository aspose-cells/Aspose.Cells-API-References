---
title: "FormatCondition.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. La valeur texte dans une règle de mise en forme conditionnelle contenant du texte. Valide uniquement pour les types containsText, notContainsText, beginsWith et endsWith. La valeur par défaut est null"
type: docs
url: /fr/net/aspose.cells/formatcondition/text/
---
## FormatCondition.Text property

La valeur texte dans une règle de mise en forme conditionnelle "text contains". Valide uniquement pour les types = containsText, notContainsText, beginsWith et endsWith. La valeur par défaut est null.

```csharp
public string Text { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTextDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter une mise en forme conditionnelle
            ConditionalFormattingCollection conditionalFormattings = sheet.ConditionalFormattings;
            int collectionIndex = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[collectionIndex];

            // Ajouter une condition de texte
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.ContainsText);
            FormatCondition formatCondition = formatConditions[conditionIndex];
            
            // Définir la propriété text (démonstration de texte russe)
            formatCondition.Text = "вс";

            // Appliquer le style de mise en forme
            Style style = formatCondition.Style;
            style.BackgroundColor = Color.Red;
            formatCondition.Style = style;

            // Appliquer à la cellule A1
            formatConditions.AddArea(CellArea.CreateCellArea("A1", "A1"));

            // Enregistrer et vérifier
            string outputPath = "FormatConditionPropertyTextDemo_Output.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("FormatCondition Text property demo completed successfully.");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


