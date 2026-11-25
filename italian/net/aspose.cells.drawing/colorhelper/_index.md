---
title: "Class ColorHelper"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ColorHelper class. Fornisce funzioni di supporto sul colore"
type: docs
url: /it/net/aspose.cells.drawing/colorhelper/
---
## ColorHelper class

Fornisce funzioni di supporto relative al colore.

```csharp
public class ColorHelper
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [FromOleColor](../../aspose.cells.drawing/colorhelper/fromolecolor/)(int) | Converti OLE_COLOR. |
| static [ToOleColor](../../aspose.cells.drawing/colorhelper/toolecolor/)(Color, Workbook) | Converti il colore in OLE_COLOR |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassColorHelperDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Converti il colore OLE in System.Drawing.Color (Verde)
            int oleGreen = 0x00FF00;
            Color colorFromOle = ColorHelper.FromOleColor(oleGreen);

            // Applica il colore convertito allo sfondo della cella A1
            Cell cellA1 = worksheet.Cells["A1"];
            Style styleA1 = cellA1.GetStyle();
            styleA1.ForegroundColor = colorFromOle;
            styleA1.Pattern = BackgroundType.Solid;
            cellA1.SetStyle(styleA1);

            // Converti System.Drawing.Color nuovamente in colore OLE
            int convertedOle = ColorHelper.ToOleColor(colorFromOle, workbook);

            // Converti il risultato OLE nuovamente in Color (verifica)
            Color colorFromConvertedOle = ColorHelper.FromOleColor(convertedOle);

            // Applica il colore riconvertito allo sfondo della cella A2
            Cell cellA2 = worksheet.Cells["A2"];
            Style styleA2 = cellA2.GetStyle();
            styleA2.ForegroundColor = colorFromConvertedOle;
            styleA2.Pattern = BackgroundType.Solid;
            cellA2.SetStyle(styleA2);

            // Salva la cartella di lavoro modificata
            workbook.Save("DrawingClassColorHelperDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


