---
title: "Classe TwoColorGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.TwoColorGradient class. Rappresenta una sfumatura a due colori"
type: docs
url: /it/net/aspose.cells/twocolorgradient/
---
## TwoColorGradient class

Rappresenta una sfumatura a due colori.

```csharp
public class TwoColorGradient
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TwoColorGradient](twocolorgradient/)(Color, Color, GradientStyleType, int) |  |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Color1](../../aspose.cells/twocolorgradient/color1/) { get; set; } | Ottiene e imposta il primo colore della sfumatura. |
| [Color2](../../aspose.cells/twocolorgradient/color2/) { get; set; } | Ottiene e imposta il secondo colore della sfumatura. |
| [GradientStyleType](../../aspose.cells/twocolorgradient/gradientstyletype/) { get; set; } | Ottiene e imposta lo stile di ombreggiatura della sfumatura. |
| [Variant](../../aspose.cells/twocolorgradient/variant/) { get; set; } | Ottiene e imposta la variante della sfumatura. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class CellsClassTwoColorGradientDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inizializza TwoColorGradient con i parametri del costruttore
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightSkyBlue, 
                Color.DarkBlue, 
                GradientStyleType.DiagonalUp, 
                2);

            // Modifica le proprietà del gradiente dopo l'inizializzazione
            gradient.GradientStyleType = GradientStyleType.DiagonalDown;

            // Crea lo stile della cella e applica il gradiente
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);

            // Applica lo stile alla cella e aggiungi il contenuto
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Aspose.Cells TwoColorGradient Demo");
            cell.SetStyle(style);

            // Regola le dimensioni della cella per la visibilità
            worksheet.Cells.SetRowHeight(1, 45);
            worksheet.Cells.SetColumnWidth(1, 55);

            // Salva il risultato con la formattazione a gradiente
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


