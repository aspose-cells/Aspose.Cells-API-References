---
title: "Worksheet.Index"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene l'indice del foglio nella collezione dei fogli di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/index/
---
## Worksheet.Index property

Ottiene l'indice del foglio nella collezione dei fogli di lavoro.

```csharp
public int Index { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi tre fogli di lavoro
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Accedi ai fogli di lavoro per indice e dimostra la proprietà Index
            Console.WriteLine("Worksheet Index Demonstration:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                Console.WriteLine($"Worksheet Name: {sheet.Name}, Index: {sheet.Index}");
            }

            // Aggiungi della formattazione condizionale per dimostrare l'uso dell'indice
            Worksheet firstSheet = workbook.Worksheets[0];
            int formatIndex = firstSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = firstSheet.ConditionalFormattings[formatIndex];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Visualizza le informazioni sull'indice della formattazione condizionale
            Console.WriteLine("\nConditional Formatting Indexes:");
            Console.WriteLine($"Worksheet Index: {firstSheet.Index}");
            Console.WriteLine($"Formatting Collection Index: {formatIndex}");
            Console.WriteLine($"First Condition Index: 0");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


