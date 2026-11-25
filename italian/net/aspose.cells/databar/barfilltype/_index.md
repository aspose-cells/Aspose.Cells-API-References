---
title: "DataBar.BarFillType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBar. Ottiene o imposta come una barra dati viene riempita con colore"
type: docs
url: /it/net/aspose.cells/databar/barfilltype/
---
## DataBar.BarFillType property

Ottiene o imposta come una barra dati è riempita di colore.

```csharp
public DataBarFillType BarFillType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarFillTypeDemo
    {
        public static void Run()
        {
            // Istanzia un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 5,
                StartColumn = 0,
                EndColumn = 5
            };
            fcs.AddArea(ca);

            // Aggiungi condizione DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Configura le proprietà DataBar
            DataBar dataBar = fc.DataBar;
            dataBar.BarFillType = DataBarFillType.Gradient; // Demonstrating BarFillType usage
            dataBar.Color = Color.Blue;

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(100);

            // Salva la cartella di lavoro
            workbook.Save("DataBarFillTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [DataBarFillType](../../databarfilltype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


