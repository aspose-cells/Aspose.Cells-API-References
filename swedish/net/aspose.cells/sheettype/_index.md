---
title: "Enum SheetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SheetType‑enum. Anger kalkylbladstypen"
type: docs
url: /sv/net/aspose.cells/sheettype/
---
## SheetType enumeration

Anger arbetsbladstypen.

```csharp
public enum SheetType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| VB | `0` | Visual Basic-modul |
| Worksheet | `1` |  |
| Chart | `2` | Diagram |
| BIFF4Macro | `3` | BIFF4-makroblad |
| InternationalMacro | `4` | Internationellt makroblad |
| Other | `5` |  |
| Dialog | `6` | Dialogarbetsblad |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSheetTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Infoga ett nytt arbetsblad av typen Worksheet på index 0
            Worksheet newWorksheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
            
            // Ange namnet på det nya arbetsbladet
            newWorksheet.Name = "InsertedSheet";
            
            // Kom åt celler i det nya arbetsbladet och lägg till lite data
            newWorksheet.Cells["A1"].PutValue("This is a new worksheet");
            
            // Spara arbetsboken
            workbook.Save("SheetTypeDemoOutput.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


