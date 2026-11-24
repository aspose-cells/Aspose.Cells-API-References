---
title: "Worksheet.HorizontalPageBreaks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die HorizontalPageBreakCollection-Sammlung zurück"
type: docs
url: /de/net/aspose.cells/worksheet/horizontalpagebreaks/
---
## Worksheet.HorizontalPageBreaks property

Gibt die [`HorizontalPageBreakCollection`](../../horizontalpagebreakcollection/) Sammlung zurück.

```csharp
public HorizontalPageBreakCollection HorizontalPageBreaks { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge horizontale Seitenumbrüche auf verschiedene Arten hinzu
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            worksheet.HorizontalPageBreaks.Add(15, 2);
            worksheet.HorizontalPageBreaks.Add("G5");

            // Entferne den ersten Seitenumbruch
            worksheet.HorizontalPageBreaks.RemoveAt(0);

            // Ausgaben speichern
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
            workbook.Save("HorizontalPageBreaksDemo.pdf");
        }
    }
}
```

### Siehe auch

* class [HorizontalPageBreakCollection](../../horizontalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


