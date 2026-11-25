---
title: "Classe DataBar"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DataBar. Descrive la regola di formattazione condizionale DataBar. Questa regola di formattazione condizionale visualizza una barra dati graduale nell'intervallo di celle"
type: docs
url: /it/net/aspose.cells/databar/
---
## DataBar class

Descrive la regola di formattazione condizionale DataBar. Questa regola di formattazione condizionale visualizza una barra dati graduale nell'intervallo di celle.

```csharp
public class DataBar
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor/) { get; set; } | Ottiene il colore dell'asse per le celle con formattazione condizionale come barre dati. |
| [AxisPosition](../../aspose.cells/databar/axisposition/) { get; set; } | Ottiene o imposta la posizione dell'asse delle barre dati specificata da una regola di formattazione condizionale. |
| [BarBorder](../../aspose.cells/databar/barborder/) { get; } | Ottiene un oggetto che specifica il bordo di una barra dati. |
| [BarFillType](../../aspose.cells/databar/barfilltype/) { get; set; } | Ottiene o imposta come una barra dati è riempita di colore. |
| [Color](../../aspose.cells/databar/color/) { get; set; } | Ottieni o imposta il colore di questa DataBar. |
| [Direction](../../aspose.cells/databar/direction/) { get; set; } | Ottiene o imposta la direzione in cui viene visualizzata la DataBar. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo/) { get; } | Ottieni o imposta l'oggetto valore massimo di questa DataBar. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Min. |
| [MaxLength](../../aspose.cells/databar/maxlength/) { get; set; } | Rappresenta la lunghezza massima della DataBar. |
| [MinCfvo](../../aspose.cells/databar/mincfvo/) { get; } | Ottieni o imposta l'oggetto valore minimo di questa DataBar. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Max. |
| [MinLength](../../aspose.cells/databar/minlength/) { get; set; } | Rappresenta la lunghezza minima della DataBar. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat/) { get; } | Ottiene l'oggetto NegativeBarFormat associato a una regola di formattazione condizionale della DataBar. |
| [ShowValue](../../aspose.cells/databar/showvalue/) { get; set; } | Ottieni o imposta il flag che indica se mostrare i valori delle celle a cui è applicata questa DataBar. Il valore predefinito è true. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage/)(Cell, ImageOrPrintOptions) | Renderizza la DataBar nella cella in un array di byte dell'immagine. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarDemo
    {
        public static void DataBarExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Aggiunge condizione
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Ottieni DataBar
            DataBar dataBar = cond.DataBar;

            // Imposta le proprietà di DataBar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Inserisci valori delle celle
            Aspose.Cells.Cell cell1 = sheet.Cells["A1"];
            cell1.PutValue(10);
            Aspose.Cells.Cell cell2 = sheet.Cells["A2"];
            cell2.PutValue(120);
            Aspose.Cells.Cell cell3 = sheet.Cells["A3"];
            cell3.PutValue(260);

            // Salvataggio del file Excel
            workbook.Save("DataBarExample.xlsx");
            workbook.Save("DataBarExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


