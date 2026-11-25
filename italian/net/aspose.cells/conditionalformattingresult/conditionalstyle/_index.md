---
title: "ConditionalFormattingResult.ConditionalStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ConditionalFormattingResult proprietà. Restituisce lo stile del risultato condizionale"
type: docs
url: /it/net/aspose.cells/conditionalformattingresult/conditionalstyle/
---
## ConditionalFormattingResult.ConditionalStyle property

Ottiene lo stile del risultato condizionale.

```csharp
public Style ConditionalStyle { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 0 });
            
            // Crea la condizione e imposta lo stile
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
            FormatCondition fc = fcc[conditionIndex];
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            fc.Style = style;

            // Ottieni la cella con formattazione condizionale
            Cell cell = worksheet.Cells["A3"];
            Style conditionalStyle = cell.GetConditionalFormattingResult().ConditionalStyle;
            
            // Emetti il colore per dimostrare la proprietà
            Console.WriteLine("Conditional Style Font Color: " + conditionalStyle.Font.Color);
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


