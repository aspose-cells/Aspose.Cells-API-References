---
title: "ConditionalFormattingResult.ConditionalStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConditionalFormattingResult. Obtient le style du résultat conditionnel"
type: docs
url: /fr/net/aspose.cells/conditionalformattingresult/conditionalstyle/
---
## ConditionalFormattingResult.ConditionalStyle property

Obtient le style du résultat conditionnel.

```csharp
public Style ConditionalStyle { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 0 });
            
            // Créez une condition et définissez le style
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
            FormatCondition fc = fcc[conditionIndex];
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            fc.Style = style;

            // Obtenez la cellule avec le formatage conditionnel
            Cell cell = worksheet.Cells["A3"];
            Style conditionalStyle = cell.GetConditionalFormattingResult().ConditionalStyle;
            
            // Affichez la couleur pour démontrer la propriété
            Console.WriteLine("Conditional Style Font Color: " + conditionalStyle.Font.Color);
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


