---
title: "Classe NegativeBarFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.NegativeBarFormat. Rappresenta le impostazioni di colore delle barre dati per valori negativi definiti da una regola di formattazione condizionale a barre dati"
type: docs
url: /it/net/aspose.cells/negativebarformat/
---
## NegativeBarFormat class

Rappresenta le impostazioni di colore delle barre dei dati per i valori negativi definiti da una regola di formattazione condizionale a barre dei dati.

```csharp
public class NegativeBarFormat
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BorderColor](../../aspose.cells/negativebarformat/bordercolor/) { get; set; } | Ottiene o imposta un oggetto FormatColor che puoi usare per specificare il colore del bordo per le barre dati negative. |
| [BorderColorType](../../aspose.cells/negativebarformat/bordercolortype/) { get; set; } | Indica se utilizzare lo stesso colore del bordo delle barre dati positive. |
| [Color](../../aspose.cells/negativebarformat/color/) { get; set; } | Ottiene o imposta un oggetto FormatColor che puoi usare per specificare il colore di riempimento per le barre dati negative. |
| [ColorType](../../aspose.cells/negativebarformat/colortype/) { get; set; } | Ottiene o imposta se utilizzare lo stesso colore di riempimento delle barre dati positive. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class NegativeBarFormatDemo
    {
        public static void NegativeBarFormatExample()
        {
            // Istanzia un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Aggiunge una condizione per DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Ottieni DataBar e imposta le sue proprietà
            DataBar dataBar = fc.DataBar;
            dataBar.Color = Color.Orange;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // Configura le proprietà di NegativeBarFormat
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = Color.White;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = Color.Yellow;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;

            // Inserisci alcuni valori nelle celle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);

            // Salva la cartella di lavoro
            workbook.Save("NegativeBarFormatExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


