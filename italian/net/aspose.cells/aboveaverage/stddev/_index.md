---
title: "AboveAverage.StdDev"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AboveAverage. Ottieni o imposta il numero di deviazioni standard da includere sopra o sotto la media nella regola di formattazione condizionale. Il valore di input deve essere compreso tra 0 e 3, inclusi 0 e 3. Impostare questo valore a 0 significa che stdDev non è impostato. Il valore predefinito è 0"
type: docs
url: /it/net/aspose.cells/aboveaverage/stddev/
---
## AboveAverage.StdDev property

Ottieni o imposta il numero di deviazioni standard da includere sopra o sotto la media nella regola di formattazione condizionale. Il valore di input deve essere compreso tra 0 e 3 (inclusi 0 e 3). Impostare questo valore a 0 significa che stdDev non è impostato. Il valore predefinito è 0.

```csharp
public int StdDev { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyStdDevDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.StdDev = 2;

            // Popola dati di esempio
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50;

            workbook.Save("AboveAverageStdDevDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


