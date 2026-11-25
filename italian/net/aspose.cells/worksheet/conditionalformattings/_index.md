---
title: "Worksheet.ConditionalFormattings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Restituisce i ConditionalFormattings nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/conditionalformattings/
---
## Worksheet.ConditionalFormattings property

Ottiene i ConditionalFormattings nel foglio di lavoro.

```csharp
public ConditionalFormattingCollection ConditionalFormattings { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyConditionalFormattingsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Crea formattazione condizionale
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Imposta l'intervallo
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Aggiungi condizione
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
            FormatCondition fc = fcc[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Red;

            // Salva la cartella di lavoro
            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingCollection](../../conditionalformattingcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


