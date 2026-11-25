---
title: "FormatCondition.ColorScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Ottieni l'istanza ColorScale della formattazione condizionale. L'istanza predefinita è un 3ColorScale verde‑giallo‑rosso. Valido solo per il tipo ColorScale"
type: docs
url: /it/net/aspose.cells/formatcondition/colorscale/
---
## FormatCondition.ColorScale property

Ottieni l'istanza "ColorScale" della formattazione condizionale. L'istanza predefinita è una "green-yellow-red" 3ColorScale. Valida solo per type = ColorScale.

```csharp
public ColorScale ColorScale { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyColorScaleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Aggiungi una formattazione condizionale a scala di colore
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Imposta l'intervallo per la formattazione condizionale
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Imposta le proprietà della scala di colori
            fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[0];
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Green;

            // Salva la cartella di lavoro
            workbook.Save("ColorScaleExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [ColorScale](../../colorscale/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


