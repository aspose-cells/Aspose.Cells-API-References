---
title: "Enum BackgroundType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.BackgroundType. Elenca i tipi di modello di sfondo della cella"
type: docs
url: /it/net/aspose.cells/backgroundtype/
---
## BackgroundType enumeration

Enumera i tipi di pattern di sfondo delle celle.

```csharp
public enum BackgroundType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DiagonalCrosshatch | `9` | Rappresenta il modello a reticolato diagonale. |
| DiagonalStripe | `8` | Rappresenta il modello a strisce diagonali. |
| Gray6 | `18` | Rappresenta il modello grigio al 6,25% |
| Gray12 | `17` | Rappresenta il modello grigio al 12,5% |
| Gray25 | `4` | Rappresenta il modello grigio al 25%. |
| Gray50 | `2` | Rappresenta il modello grigio al 50%. |
| Gray75 | `3` | Rappresenta il modello grigio al 75%. |
| HorizontalStripe | `5` | Rappresenta il modello a strisce orizzontali. |
| None | `0` | Rappresenta nessuno sfondo. |
| ReverseDiagonalStripe | `7` | Rappresenta il modello a strisce diagonali inverse. |
| Solid | `1` | Rappresenta il modello solido. |
| ThickDiagonalCrosshatch | `10` | Rappresenta il modello a reticolato diagonale spesso. |
| ThinDiagonalCrosshatch | `16` | Rappresenta il modello a reticolato diagonale sottile. |
| ThinDiagonalStripe | `14` | Rappresenta il modello a strisce diagonali sottili. |
| ThinHorizontalCrosshatch | `15` | Rappresenta il modello a reticolato orizzontale sottile. |
| ThinHorizontalStripe | `11` | Rappresenta il modello a strisce orizzontali sottili. |
| ThinReverseDiagonalStripe | `13` | Rappresenta il modello a strisce diagonali inverse sottili. |
| ThinVerticalStripe | `12` | Rappresenta un modello di strisce verticali sottili. |
| VerticalStripe | `6` | Rappresenta un modello di strisce verticali. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BackgroundTypeDemo
    {
        public static void BackgroundTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro nella cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi a una cella dal foglio di lavoro
            Cell cell = worksheet.Cells["A1"];
            
            // Imposta il valore della cella
            cell.PutValue("Hello, Aspose!");

            // Crea un oggetto stile
            Style style = cell.GetStyle();
            
            // Imposta il tipo di modello di sfondo
            style.Pattern = BackgroundType.DiagonalStripe;
            
            // Imposta il colore di primo piano
            style.ForegroundColor = Color.Red;
            
            // Imposta il colore di sfondo
            style.BackgroundColor = Color.Green;
            
            // Applica lo stile alla cella
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("BackgroundTypeExample.xlsx");
            workbook.Save("BackgroundTypeExample.pdf");



        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


