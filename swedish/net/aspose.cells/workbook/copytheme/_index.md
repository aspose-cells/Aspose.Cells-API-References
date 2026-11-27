---
title: "Workbook.CopyTheme"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Kopierar temat från en annan arbetsbok"
type: docs
url: /sv/net/aspose.cells/workbook/copytheme/
---
## Workbook.CopyTheme method

Kopierar temat från en annan Workbook.

```csharp
public void CopyTheme(Workbook source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Arbetsbok | Källarbetsbok. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyThemeWithWorkbookDemo
    {
        public static void Run()
        {
            // Skapa källarbetsbok (temat sätts automatiskt när en mallfil öppnas)
            Workbook sourceWorkbook = new Workbook(FileFormatType.Xlsx);

            // Skapa målarbetsbok
            Workbook destWorkbook = new Workbook();
            
            // Kopiera tema från käll- till destinationsarbetsbok
            destWorkbook.CopyTheme(sourceWorkbook);

            // Spara målarbetsboken
            destWorkbook.Save("output_with_theme.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


