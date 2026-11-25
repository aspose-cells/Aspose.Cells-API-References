---
title: "Classe ConditionalFormattingResult"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ConditionalFormattingResult. Rappresenta il risultato della formattazione condizionale che si applica a una cella"
type: docs
url: /it/net/aspose.cells/conditionalformattingresult/
---
## ConditionalFormattingResult class

Rappresenta il risultato della formattazione condizionale che si applica a una cella.

```csharp
public class ConditionalFormattingResult
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ColorScaleResult](../../aspose.cells/conditionalformattingresult/colorscaleresult/) { get; } | Ottiene il colore di visualizzazione della scala di colori. |
| [ConditionalFormattingColorScale](../../aspose.cells/conditionalformattingresult/conditionalformattingcolorscale/) { get; } | Ottiene l'oggetto ColorScale. |
| [ConditionalFormattingDataBar](../../aspose.cells/conditionalformattingresult/conditionalformattingdatabar/) { get; } | Ottiene l'oggetto DataBar. |
| [ConditionalFormattingIcon](../../aspose.cells/conditionalformattingresult/conditionalformattingicon/) { get; } | Ottiene l'immagine del set di icone. |
| [ConditionalStyle](../../aspose.cells/conditionalformattingresult/conditionalstyle/) { get; } | Ottiene lo stile del risultato condizionale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingResultDemo
    {
        public static void ConditionalFormattingResultExample()
        {
            // Istanzia un oggetto cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Aggiunge condizione
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Imposta le proprietà di ColorScale
            fc.ColorScale.Is3ColorScale = true;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxColor = Color.Green;

            // Applica alcuni valori alle celle
            for (int i = 0; i <= 10; i++)
            {
                for (int j = 0; j <= 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Ottieni il risultato della formattazione condizionale per una cella specifica
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult cfr = cell.GetConditionalFormattingResult();

            // Accedi alle proprietà di ConditionalFormattingResult
            Style conditionalStyle = cfr.ConditionalStyle;
            ConditionalFormattingIcon icon = cfr.ConditionalFormattingIcon;
            DataBar dataBar = cfr.ConditionalFormattingDataBar;
            ColorScale colorScale = cfr.ConditionalFormattingColorScale;
            Color colorScaleResult = cfr.ColorScaleResult;

            // Visualizza alcune delle proprietà
            Console.WriteLine("Conditional Style Background Color: " + (conditionalStyle != null ? conditionalStyle.BackgroundColor : Color.Empty));
            Console.WriteLine("Conditional Formatting Icon Type: " + (icon != null ? icon.Type.ToString() : "No Icon"));
            Console.WriteLine("Conditional Formatting DataBar Color: " + (dataBar != null ? dataBar.Color.ToString() : "No DataBar"));
            Console.WriteLine("Conditional Formatting ColorScale Min Color: " + (colorScale != null ? colorScale.MinColor.ToString() : "No ColorScale"));
            Console.WriteLine("Color Scale Result: " + colorScaleResult);

            // Salva la cartella di lavoro
            workbook.Save("ConditionalFormattingResultExample.xlsx");
            workbook.Save("ConditionalFormattingResultExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


