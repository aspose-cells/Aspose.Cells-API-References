---
title: "Enum TextDirectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.TextDirectionType enum. Rappresenta la direzione del flusso di testo per questo paragrafo"
type: docs
url: /it/net/aspose.cells/textdirectiontype/
---
## TextDirectionType enumeration

Rappresenta la direzione del flusso di testo per questo paragrafo.

```csharp
public enum TextDirectionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Context | `0` |  |
| LeftToRight | `1` |  |
| RightToLeft | `2` |  |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTextDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta la direzione del testo da destra a sinistra
            Style style = cells["A1"].GetStyle();
            style.TextDirection = TextDirectionType.RightToLeft;
            cells["A1"].SetStyle(style);
            cells["A1"].PutValue("Right to Left Text");

            // Imposta la direzione del testo da sinistra a destra
            style = cells["A2"].GetStyle();
            style.TextDirection = TextDirectionType.LeftToRight;
            cells["A2"].SetStyle(style);
            cells["A2"].PutValue("Left to Right Text");

            // Imposta la direzione del testo del contesto
            style = cells["A3"].GetStyle();
            style.TextDirection = TextDirectionType.Context;
            cells["A3"].SetStyle(style);
            cells["A3"].PutValue("Context Text Direction");

            workbook.Save("TextDirectionTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


