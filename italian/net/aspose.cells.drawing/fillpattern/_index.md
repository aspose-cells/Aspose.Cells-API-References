---
title: "Enum FillPattern"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.FillPattern enum. Elenca i tipi di modello di riempimento della forma"
type: docs
url: /it/net/aspose.cells.drawing/fillpattern/
---
## FillPattern enumeration

Enumera i tipi di modello di riempimento della forma.

```csharp
public enum FillPattern
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Rappresenta nessuno sfondo. |
| Solid | `1` | Rappresenta il modello solido. |
| Gray5 | `2` | Rappresenta il modello grigio al 5%. |
| Gray10 | `3` | Rappresenta il modello grigio al 10%. |
| Gray20 | `4` | Rappresenta il modello grigio al 20%. |
| Gray30 | `5` | Rappresenta il modello grigio al 30%. |
| Gray40 | `6` | Rappresenta il modello grigio al 40%. |
| Gray50 | `7` | Rappresenta il modello grigio al 50%. |
| Gray60 | `8` | Rappresenta il modello grigio al 60%. |
| Gray70 | `9` | Rappresenta il modello grigio al 70%. |
| Gray75 | `10` | Rappresenta il modello grigio al 75%. |
| Gray80 | `11` | Rappresenta il motivo grigio al 80%. |
| Gray90 | `12` | Rappresenta il motivo grigio al 90%. |
| Gray25 | `13` | Rappresenta il modello grigio al 25%. |
| LightDownwardDiagonal | `14` | Rappresenta il motivo diagonale discendente chiaro. |
| LightUpwardDiagonal | `15` | Rappresenta il motivo diagonale ascendente chiaro. |
| DarkDownwardDiagonal | `16` | Rappresenta il motivo diagonale discendente scuro. |
| DarkUpwardDiagonal | `17` | Rappresenta il motivo diagonale ascendente scuro. |
| WideDownwardDiagonal | `18` | Rappresenta il motivo diagonale discendente largo. |
| WideUpwardDiagonal | `19` | Rappresenta il motivo diagonale ascendente largo. |
| LightVertical | `20` | Rappresenta il motivo verticale chiaro. |
| LightHorizontal | `21` | Rappresenta il motivo orizzontale chiaro. |
| NarrowVertical | `22` | Rappresenta il motivo verticale stretto. |
| NarrowHorizontal | `23` | Rappresenta il motivo orizzontale stretto. |
| DarkVertical | `24` | Rappresenta il motivo verticale scuro. |
| DarkHorizontal | `25` | Rappresenta il motivo orizzontale scuro. |
| DashedDownwardDiagonal | `26` | Rappresenta il motivo diagonale discendente tratteggiato. |
| DashedUpwardDiagonal | `27` | Rappresenta il motivo diagonale ascendente tratteggiato. |
| DashedVertical | `28` | Rappresenta il motivo verticale tratteggiato. |
| DashedHorizontal | `29` | Rappresenta il motivo orizzontale tratteggiato. |
| SmallConfetti | `30` | Rappresenta il motivo confetti piccolo. |
| LargeConfetti | `31` | Rappresenta il motivo confetti grande. |
| ZigZag | `32` | Rappresenta il motivo a zig zag. |
| Wave | `33` | Rappresenta il motivo a onde. |
| DiagonalBrick | `34` | Rappresenta il motivo a mattoni diagonali. |
| HorizontalBrick | `35` | Rappresenta il motivo a mattoni orizzontali. |
| Weave | `36` | Rappresenta il motivo intrecciato. |
| Plaid | `37` | Rappresenta il motivo a quadri. |
| Divot | `38` | Rappresenta il motivo a incavo. |
| DottedGrid | `39` | Rappresenta il motivo a griglia puntinata. |
| DottedDiamond | `40` | Rappresenta il motivo a diamante puntinato. |
| Shingle | `41` | Rappresenta il motivo a tegole. |
| Trellis | `42` | Rappresenta il motivo a traliccio. |
| Sphere | `43` | Rappresenta il motivo a sfera. |
| SmallGrid | `44` | Rappresenta il motivo a griglia piccola. |
| LargeGrid | `45` | Rappresenta il motivo a griglia grande. |
| SmallCheckerBoard | `46` | Rappresenta il motivo a scacchiera piccola. |
| LargeCheckerBoard | `47` | Rappresenta il motivo a scacchiera grande. |
| OutlinedDiamond | `48` | Rappresenta il motivo a diamante contornato. |
| SolidDiamond | `49` | Rappresenta il motivo a diamante pieno. |
| Unknown | `50` | Rappresenta un motivo sconosciuto. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillPatternDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta il motivo di riempimento per la prima serie
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Plaid;

            // Salva la cartella di lavoro
            workbook.Save("FillPatternDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


