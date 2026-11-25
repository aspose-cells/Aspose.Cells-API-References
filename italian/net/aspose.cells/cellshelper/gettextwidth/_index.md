---
title: "CellsHelper.GetTextWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Ottieni la larghezza del testo in unità di punti"
type: docs
url: /it/net/aspose.cells/cellshelper/gettextwidth/
---
## CellsHelper.GetTextWidth method

Ottiene la larghezza del testo in unità di punti.

```csharp
public static double GetTextWidth(string text, Font font, double scaling)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | Il testo. |
| font | Font | Il font del testo. |
| scalatura | Double | La scalatura del testo. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetTextWidthWithStringFontDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Font font = workbook.DefaultStyle.Font;
            double textWidth = CellsHelper.GetTextWidth("Sample Text", font, 1.0);
            Console.WriteLine("Text width: " + textWidth);
        }
    }
}
```

### Vedi anche

* class [Font](../../font/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


