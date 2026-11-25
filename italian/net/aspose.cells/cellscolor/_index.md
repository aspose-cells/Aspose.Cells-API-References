---
title: "Classe CellsColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CellsColor. Rappresenta tutti i tipi di colore"
type: docs
url: /it/net/aspose.cells/cellscolor/
---
## CellsColor class

Rappresenta tutti i tipi di colore.

```csharp
public class CellsColor
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Argb](../../aspose.cells/cellscolor/argb/) { get; set; } | Ottiene e imposta il colore da un valore ARGB a 32 bit. |
| [Color](../../aspose.cells/cellscolor/color/) { get; set; } | Ottiene e imposta il colore RGB. |
| [ColorIndex](../../aspose.cells/cellscolor/colorindex/) { get; set; } | Ottiene e imposta l'indice del colore nella tavolozza dei colori. Si applica solo ai colori indicizzati. |
| [IsShapeColor](../../aspose.cells/cellscolor/isshapecolor/) { get; set; } | Ottiene e imposta il colore da applicare alla cella o alla forma. |
| [ThemeColor](../../aspose.cells/cellscolor/themecolor/) { get; set; } | Ottiene il colore del tema. Si applica solo al tipo di colore del tema. |
| [Transparency](../../aspose.cells/cellscolor/transparency/) { get; set; } | Ottiene e imposta la trasparenza come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [Type](../../aspose.cells/cellscolor/type/) { get; } | Il tipo di colore. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetTintOfShapeColor](../../aspose.cells/cellscolor/settintofshapecolor/)(double) | Imposta la tinta del colore della forma |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorDemo
    {
        public static void CellsColorExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo di celle
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A10");

            // Crea un'istanza di CellsColor
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Imposta le proprietà di CellsColor
            cellsColor.IsShapeColor = false;
            cellsColor.Color = Color.Red;
            cellsColor.ColorIndex = 5;
            cellsColor.Argb = Color.Blue.ToArgb();
            cellsColor.Transparency = 0.5;

            // Applica CellsColor all'intervallo
            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Salva la cartella di lavoro
            workbook.Save("CellsColorExample.xlsx");
            workbook.Save("CellsColorExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


