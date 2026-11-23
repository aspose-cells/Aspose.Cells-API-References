---
title: "ConditionalFormattingCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConditionalFormattingCollection. Obtient l'élément FormatConditions à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/conditionalformattingcollection/item/
---
## ConditionalFormattingCollection indexer

Obtient l'élément FormatConditions à l'index spécifié.

```csharp
public FormatConditionCollection this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Ajouter une mise en forme conditionnelle
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
            
            // Ajoutez une condition de format
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "50");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Accéder et démontrer l'utilisation de la propriété Item
            FormatConditionCollection firstFormatting = sheet.ConditionalFormattings[0];
            Console.WriteLine($"First formatting has {firstFormatting.Count} conditions");
            Console.WriteLine($"First condition operator: {firstFormatting[0].Operator}");
        }
    }
}
```

### Voir aussi

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


