---
title: "FormatCondition.AboveAverage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Ottieni l'istanza AboveAverage della formattazione condizionale. La regola predefinita dell'istanza evidenzia le celle che sono sopra la media per tutti i valori nell'intervallo. Valida solo per il tipo AboveAverage"
type: docs
url: /it/net/aspose.cells/formatcondition/aboveaverage/
---
## FormatCondition.AboveAverage property

Ottieni l'istanza "AboveAverage" della formattazione condizionale. La regola dell'istanza predefinita evidenzia le celle che sono al di sopra della media per tutti i valori nell'intervallo. Valida solo per type = AboveAverage.

```csharp
public AboveAverage AboveAverage { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyAboveAverageDemo
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
            worksheet.Cells["A5"].PutValue(50);

            // Aggiungi formattazione condizionale sopra la media
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 4, EndColumn = 0 });

            // Imposta per evidenziare i valori sopra la media
            FormatCondition fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = true;
            fc.Style.BackgroundColor = Color.Yellow;

            // Aggiungi formattazione condizionale sotto la media
            index = worksheet.ConditionalFormattings.Add();
            fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 1, EndRow = 4, EndColumn = 1 });

            // Imposta per evidenziare i valori sotto la media
            fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = false;
            fc.Style.BackgroundColor = Color.LightBlue;

            // Salva la cartella di lavoro
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AboveAverage](../../aboveaverage/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


