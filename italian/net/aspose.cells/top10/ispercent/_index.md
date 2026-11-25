---
title: "Top10.IsPercent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Top10. Ottieni o imposta se una regola top/bottom n è una regola top/bottom n percentuale. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/top10/ispercent/
---
## Top10.IsPercent property

Ottieni o imposta se una regola "top/bottom n" è una regola "top/bottom n percent". Il valore predefinito è false.

```csharp
public bool IsPercent { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsPercentDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Aggiungi una regola di formattazione condizionale Top10
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);

            // Ottieni la condizione di formattazione Top10
            FormatCondition fc = fcc[0];
            
            // Imposta le proprietà Top10
            fc.Top10.IsPercent = true;  // Demonstrate IsPercent property
            fc.Top10.IsBottom = false;
            fc.Top10.Rank = 3;

            // Applica lo stile di formattazione
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Salva la cartella di lavoro
            workbook.Save("Top10IsPercentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


