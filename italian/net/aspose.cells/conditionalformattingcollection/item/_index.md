---
title: "ConditionalFormattingCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConditionalFormattingCollection. Ottiene l'elemento FormatConditions all'indice specificato"
type: docs
url: /it/net/aspose.cells/conditionalformattingcollection/item/
---
## ConditionalFormattingCollection indexer

Restituisce l'elemento FormatConditions all'indice specificato.

```csharp
public FormatConditionCollection this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Esempi

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

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Aggiungi formattazione condizionale
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
            
            // Aggiungi condizione di formato
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "50");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Accedi e dimostra l'uso della proprietà Item
            FormatConditionCollection firstFormatting = sheet.ConditionalFormattings[0];
            Console.WriteLine($"First formatting has {firstFormatting.Count} conditions");
            Console.WriteLine($"First condition operator: {firstFormatting[0].Operator}");
        }
    }
}
```

### Vedi anche

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


