---
title: "FormatCondition.Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Ottiene o imposta lo stile degli intervalli di celle formattate condizionalmente"
type: docs
url: /it/net/aspose.cells/formatcondition/style/
---
## FormatCondition.Style property

Ottiene o imposta lo stile degli intervalli di celle formattate condizionalmente.

```csharp
public Style Style { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStyleDemo
    {
        public static void Run()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(30);
            worksheet.Cells["A2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(90);

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Imposta l'intervallo
            CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(area);

            // Aggiungi la prima condizione (valori tra 40-80)
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "40", "80");
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Yellow;
            fc1.Style.Font.Color = System.Drawing.Color.Black;

            // Aggiungi la seconda condizione (valori > 80)
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "80", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;
            fc2.Style.Font.Color = System.Drawing.Color.White;
            fc2.Style.Font.IsBold = true;

            // Salva la cartella di lavoro
            workbook.Save("FormatConditionStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


