---
title: "Enum DataBarFillType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.DataBarFillType. Specifica come una barra dei dati è riempita con colore"
type: docs
url: /it/net/aspose.cells/databarfilltype/
---
## DataBarFillType enumeration

Specifica come una barra dei dati viene riempita con colore.

```csharp
public enum DataBarFillType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Solid | `0` | La barra dei dati è riempita con colore solido. |
| Gradient | `1` | La barra dei dati è riempita con una sfumatura di colore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarFillTypeDemo
    {
        public static void DataBarFillTypeExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Aggiunta di un nuovo foglio di lavoro al Workbook
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale.
            CellArea ca = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Aggiunge condizione
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Ottieni Databar
            DataBar dataBar = cond.DataBar;

            // Imposta le proprietà di Databar
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
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Salvataggio del file Excel
            workbook.Save("DataBarFillTypeExample.xlsx");
            workbook.Save("DataBarFillTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


