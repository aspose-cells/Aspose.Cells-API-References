---
title: "Enum FillType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.FillType enum. Tipo di formato di riempimento"
type: docs
url: /it/net/aspose.cells.drawing/filltype/
---
## FillType enumeration

Tipo di formato di riempimento.

```csharp
public enum FillType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Rappresenta il tipo di formattazione automatica. |
| None | `1` | Rappresenta il tipo di formattazione nessuna. |
| Solid | `2` | Formato di riempimento solido. |
| Gradient | `3` | Formato di riempimento a gradiente. |
| Texture | `4` | Formato di riempimento a trama (include il riempimento immagine). |
| Pattern | `5` | Formato di riempimento a motivo. |
| Group | `6` | Eredita le proprietà di riempimento del gruppo. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 150);
            
            // Imposta il tipo di riempimento sfumato
            rectangle.Fill.FillType = FillType.Gradient;
            rectangle.Fill.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            // Aggiungi una casella di testo
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 10, 10, 100, 150);
            textBox.Text = "Gradient Fill Example";
            
            // Imposta il tipo di riempimento gradiente per la casella di testo
            textBox.Fill.FillType = FillType.Gradient;
            textBox.Fill.SetTwoColorGradient(Color.LightGreen, Color.DarkGreen, GradientStyleType.Vertical, 1);

            // Salva la cartella di lavoro
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


