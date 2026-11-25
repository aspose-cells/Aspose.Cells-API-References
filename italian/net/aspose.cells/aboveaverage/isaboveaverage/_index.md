---
title: "AboveAverage.IsAboveAverage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AboveAverage. Ottieni o imposta il flag che indica se la regola è una regola sopra la media. true indica sopra la media. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/aboveaverage/isaboveaverage/
---
## AboveAverage.IsAboveAverage property

Ottieni o imposta il flag che indica se la regola è una regola "sopra la media". 'true' indica "sopra la media". Il valore predefinito è true.

```csharp
public bool IsAboveAverage { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsAboveAverageDemo
    {
        public static void Run()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();
            
            // Ottieni il primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per dimostrare la formattazione condizionale
            for (int i = 0; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Aggiungi una formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Aggiungi una condizione AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Configura le proprietà AboveAverage
            fc.AboveAverage.IsAboveAverage = true;  // Highlight values above average
            fc.AboveAverage.IsEqualAverage = false; // Exclude values equal to average

            // Salva il file Excel
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


