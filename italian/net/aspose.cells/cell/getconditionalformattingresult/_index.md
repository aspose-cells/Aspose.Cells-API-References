---
title: "Cell.GetConditionalFormattingResult"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottieni il risultato della formattazione condizionale"
type: docs
url: /it/net/aspose.cells/cell/getconditionalformattingresult/
---
## Cell.GetConditionalFormattingResult method

Ottieni il risultato della formattazione condizionale.

```csharp
public ConditionalFormattingResult GetConditionalFormattingResult()
```

### Osservazioni

Restituisce null se nessuna formattazione condizionale è applicata a questa cella,

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetConditionalFormattingResultDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            // Imposta condizione e stile
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fcc[conditionIndex].Style = style;

            // Ottieni il risultato della formattazione condizionale per una cella
            Cell cell = worksheet.Cells["A2"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            // Risultato di output
            Console.WriteLine("Cell A2 meets condition: " + (result.ConditionalStyle != null));
            Console.WriteLine("Applied font color: " + result.ConditionalStyle.Font.Color);
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingResult](../../conditionalformattingresult/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


