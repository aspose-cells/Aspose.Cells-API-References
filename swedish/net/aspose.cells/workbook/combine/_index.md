---
title: "Workbook.Combine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Kombinerar ett annat Workbook‑objekt"
type: docs
url: /sv/net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

Kombinerar ett annat Workbook-objekt.

```csharp
public void Combine(Workbook secondWorkbook)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| secondWorkbook | Arbetsbok | Ett annat Workbook‑objekt. |

### Anmärkningar

Slå samman Excel-, ODS-, CSV- och andra filer till en fil.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCombineWithWorkbookDemo
    {
        public static void Run()
        {
            // Skapa källarbok
            Workbook sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets[0].Cells["A1"].PutValue("Source Data");

            // Skapa målarbetsbok
            Workbook destWorkbook = new Workbook(FileFormatType.Xlsx);
            destWorkbook.Worksheets[0].Cells["B2"].PutValue("Destination Data");

            // Kombinera arbetsböckerna
            destWorkbook.Combine(sourceWorkbook);

            // Spara den kombinerade arbetsboken.
            destWorkbook.Save("CombinedWorkbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


