---
title: "ColorScale.MinColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ColorScale. Ottieni o imposta il colore gradiente per il valore minimo nell'intervallo"
type: docs
url: /it/net/aspose.cells/colorscale/mincolor/
---
## ColorScale.MinColor property

Ottieni o imposta il colore gradiente per il valore minimo nell'intervallo.

```csharp
public Color MinColor { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinColorDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Crea un oggetto CellArea invece di usare una stringa
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcs.AddArea(area);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Configura la scala di colori
            ColorScale colorScale = fc.ColorScale;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Imposta i tipi di valore
            colorScale.MinCfvo.Type = FormatConditionValueType.Min;
            colorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            colorScale.MidCfvo.Value = 50;
            colorScale.MaxCfvo.Type = FormatConditionValueType.Max;

            // Salva la cartella di lavoro
            workbook.Save("ColorScaleMinColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


