---
title: "FormatCondition.Priority"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. La priorità di questa regola di formattazione condizionale. Questo valore è usato per determinare quale formato deve essere valutato e renderizzato. I valori numerici più bassi hanno priorità più alta rispetto a valori più alti, dove 1 è la priorità più alta"
type: docs
url: /it/net/aspose.cells/formatcondition/priority/
---
## FormatCondition.Priority property

La priorità di questa regola di formattazione condizionale. Questo valore è usato per determinare quale formato deve essere valutato e renderizzato. Valori numerici più bassi hanno priorità più alta rispetto a valori numerici più alti, dove '1' è la priorità più alta.

```csharp
public int Priority { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyPriorityDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Aggiungi formattazione condizionale
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            
            // Aggiungi condizioni
            int conditionIndex1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "2", "5");
            int conditionIndex2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "6", "9");

            // Imposta le priorità
            formatConditions[conditionIndex1].Priority = 2;
            formatConditions[conditionIndex2].Priority = 1;

            // Dimostra l'uso della proprietà Priority
            Console.WriteLine("Condition 1 Priority: " + formatConditions[conditionIndex1].Priority);
            Console.WriteLine("Condition 2 Priority: " + formatConditions[conditionIndex2].Priority);

            // Salva la cartella di lavoro
            workbook.Save("ConditionalFormattingPriorityDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


