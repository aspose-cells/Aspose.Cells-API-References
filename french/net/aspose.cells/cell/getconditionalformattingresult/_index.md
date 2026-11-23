---
title: "Cell.GetConditionalFormattingResult"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtenir le résultat du formatage conditionnel"
type: docs
url: /fr/net/aspose.cells/cell/getconditionalformattingresult/
---
## Cell.GetConditionalFormattingResult method

Obtenir le résultat du formatage conditionnel.

```csharp
public ConditionalFormattingResult GetConditionalFormattingResult()
```

### Remarques

Renvoie null si aucun formatage conditionnel n'est appliqué à cette cellule,

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetConditionalFormattingResultDemo
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
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            // Définir la condition et le style
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fcc[conditionIndex].Style = style;

            // Obtenir le résultat du formatage conditionnel pour une cellule
            Cell cell = worksheet.Cells["A2"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            // Résultat de sortie
            Console.WriteLine("Cell A2 meets condition: " + (result.ConditionalStyle != null));
            Console.WriteLine("Applied font color: " + result.ConditionalStyle.Font.Color);
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingResult](../../conditionalformattingresult/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


