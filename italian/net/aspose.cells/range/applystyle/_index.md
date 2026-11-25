---
title: "Range.ApplyStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Applica formati per un intero intervallo"
type: docs
url: /it/net/aspose.cells/range/applystyle/
---
## Range.ApplyStyle method

Applica formati a un intero intervallo.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | L'oggetto stile che verrà applicato. |
| flag | StyleFlag | Flag che indicano le proprietà di formattazione applicate. |

### Osservazioni

Ogni cella in questo intervallo conterrà un oggetto [`Style`](../../style/). Quindi questo è un metodo che consuma molta memoria. Si prega di usarlo con attenzione.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;

            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue("Sample text for style demonstration");

            Aspose.Cells.Range range = cells.CreateRange(0, 0, 1, 3);

            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HorizontalAlignment = true;
            styleFlag.VerticalAlignment = true;
            styleFlag.WrapText = true;

            range.ApplyStyle(style, styleFlag);

            workbook.Save("ApplyStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


