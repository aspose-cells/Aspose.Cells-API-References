---
title: "ColorScale.MaxColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ColorScale. Ottieni o imposta il colore gradiente per il valore massimo nell'intervallo"
type: docs
url: /it/net/aspose.cells/colorscale/maxcolor/
---
## ColorScale.MaxColor property

Ottieni o imposta il colore gradiente per il valore massimo nell'intervallo.

```csharp
public Color MaxColor { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMaxColorDemo
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
            worksheet.Cells["A5"].PutValue(50);

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Crea un oggetto CellArea invece di usare una stringa
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Aggiungi una condizione di scala di colori
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];
            ColorScale colorScale = fc.ColorScale;

            // Configura la scala di colori
            colorScale.Is3ColorScale = false; // Use 2-color scale for simplicity
            colorScale.MinColor = Color.Green;
            colorScale.MaxColor = Color.Red; // Demonstrating MaxColor property

            // Imposta gli oggetti valore
            colorScale.MinCfvo.Type = FormatConditionValueType.Min;
            colorScale.MaxCfvo.Type = FormatConditionValueType.Max;

            // Salva la cartella di lavoro
            workbook.Save("ColorScaleMaxColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


