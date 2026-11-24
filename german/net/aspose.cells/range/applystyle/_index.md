---
title: "Range.ApplyStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Wendet Formate auf einen gesamten Bereich an"
type: docs
url: /de/net/aspose.cells/range/applystyle/
---
## Range.ApplyStyle method

Wendet Formate für einen gesamten Bereich an.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Das Stil‑Objekt, das angewendet wird. |
| Flag | StyleFlag | Flags, die die angewendeten Formatierungseigenschaften angeben. |

### Hinweise

Jede Zelle in diesem Bereich enthält ein [`Style`](../../style/)-Objekt. Daher ist dies eine speicherintensive Methode. Bitte verwenden Sie sie vorsichtig.

### Beispiele

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

### Siehe auch

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


