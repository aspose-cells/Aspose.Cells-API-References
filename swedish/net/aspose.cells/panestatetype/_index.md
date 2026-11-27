---
title: "Enum PaneStateType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PaneStateType-enum. Representerar tillståndet för bladets panel"
type: docs
url: /sv/net/aspose.cells/panestatetype/
---
## PaneStateType enumeration

Representerar tillståndet för bladets ruta.

```csharp
public enum PaneStateType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Frozen | `0` | Panelerna är frysta, men var inte frysta innan de frystes. |
| FrozenSplit | `1` | Panelerna är frysta och delades innan de frystes. |
| Split | `2` | Panelerna är delade, men inte frysta. |
| Normal | `3` | Panelerna är varken frysta eller delade. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PaneStateTypeDemo
    {
        public static void PaneStateTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange några exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Data 1");
            worksheet.Cells["A2"].PutValue("Data 2");
            worksheet.Cells["A3"].PutValue("Data 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Frys paneler vid cell B2
            worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column

            // Kontrollera panelens tillstånd
            PaneStateType paneState = worksheet.PaneState;

            // Skriv ut panelens tillstånd
            Console.WriteLine("Current Pane State: " + paneState);

            // Spara arbetsboken
            workbook.Save("PaneStateTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


