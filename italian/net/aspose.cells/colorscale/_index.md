---
title: "Classe ColorScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ColorScale classe. Descrivi la regola di formattazione condizionale ColorScale. Questa regola di formattazione condizionale crea una scala di colori graduale sulle celle"
type: docs
url: /it/net/aspose.cells/colorscale/
---
## ColorScale class

Descrive la regola di formattazione condizionale ColorScale. Questa regola di formattazione condizionale crea una scala di colori graduale sulle celle.

```csharp
public class ColorScale
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Is3ColorScale](../../aspose.cells/colorscale/is3colorscale/) { get; set; } | Indica se la formattazione condizionale è a scala di 3 colori. |
| [MaxCfvo](../../aspose.cells/colorscale/maxcfvo/) { get; } | Ottieni o imposta l'oggetto valore massimo di questo ColorScale. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Min su di esso. |
| [MaxColor](../../aspose.cells/colorscale/maxcolor/) { get; set; } | Ottieni o imposta il colore gradiente per il valore massimo nell'intervallo. |
| [MidCfvo](../../aspose.cells/colorscale/midcfvo/) { get; } | Ottieni o imposta l'oggetto valore medio di questo ColorScale. Non è possibile impostare CFValueObject con tipo FormatConditionValueType.Max o FormatConditionValueType.Min su di esso. |
| [MidColor](../../aspose.cells/colorscale/midcolor/) { get; set; } | Ottieni o imposta il colore gradiente per il valore intermedio nell'intervallo. |
| [MinCfvo](../../aspose.cells/colorscale/mincfvo/) { get; } | Ottieni o imposta l'oggetto valore minimo di questo ColorScale. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Max su di esso. |
| [MinColor](../../aspose.cells/colorscale/mincolor/) { get; set; } | Ottieni o imposta il colore gradiente per il valore minimo nell'intervallo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColorScaleDemo
    {
        public static void ColorScaleExample()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Aggiungi una regola di formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 9 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Accedi all'oggetto ColorScale
            ColorScale colorScale = fc.ColorScale;

            // Imposta le proprietà per il ColorScale
            colorScale.Is3ColorScale = true;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Imposta gli oggetti valore minimo, medio e massimo
            ConditionalFormattingValue minCfvo = colorScale.MinCfvo;
            minCfvo.Type = FormatConditionValueType.Min;
            minCfvo.Value = null;

            ConditionalFormattingValue midCfvo = colorScale.MidCfvo;
            midCfvo.Type = FormatConditionValueType.Percentile;
            midCfvo.Value = 50;

            ConditionalFormattingValue maxCfvo = colorScale.MaxCfvo;
            maxCfvo.Type = FormatConditionValueType.Max;
            maxCfvo.Value = null;

            // Salva la cartella di lavoro
            workbook.Save("ColorScaleExample.xlsx");
            workbook.Save("ColorScaleExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


