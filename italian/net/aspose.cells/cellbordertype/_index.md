---
title: "Enum CellBorderType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.CellBorderType enum. Elenca i tipi di bordo delle celle"
type: docs
url: /it/net/aspose.cells/cellbordertype/
---
## CellBorderType enumeration

Enumera il tipo di bordo di una cella.

```csharp
public enum CellBorderType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DashDot | `9` | Rappresenta una linea sottile tratteggiata-puntinata. |
| DashDotDot | `11` | Rappresenta una linea sottile tratteggiata-punto-puntinata. |
| Dashed | `3` | Rappresenta una linea tratteggiata. |
| Dotted | `4` | Rappresenta una linea tratteggiata. |
| Double | `6` | Rappresenta una linea doppia. |
| Hair | `7` | Rappresenta una linea sottile. |
| MediumDashDot | `10` | Rappresenta una linea media tratteggiata-puntinata. |
| MediumDashDotDot | `12` | Rappresenta una linea media tratteggiata-punto-puntinata. |
| MediumDashed | `8` | Rappresenta una linea media tratteggiata. |
| None | `0` | Rappresenta nessuna linea. |
| Medium | `2` | Rappresenta una linea media. |
| SlantedDashDot | `13` | Rappresenta una linea media inclinata tratteggiata-puntinata. |
| Thick | `5` | Rappresenta una linea spessa. |
| Thin | `1` | Rappresenta una linea sottile. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellBorderTypeDemo
    {
        public static void CellBorderTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo (A1:D4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Ottieni lo stile dell'intervallo
            Style style = workbook.CreateStyle();

            // Imposta diversi stili di bordo per l'intervallo
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = Color.Black;

            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;

            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.LeftBorder].Color = Color.Green;

            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            style.Borders[BorderType.RightBorder].Color = Color.Red;

            // Applica lo stile all'intervallo
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            range.ApplyStyle(style, styleFlag);

            // Salva la cartella di lavoro
            workbook.Save("CellBorderTypeExample.xlsx");
            workbook.Save("CellBorderTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


