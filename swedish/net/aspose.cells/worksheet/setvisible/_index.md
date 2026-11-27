---
title: "Worksheet.SetVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Ställer in de synliga alternativen"
type: docs
url: /sv/net/aspose.cells/worksheet/setvisible/
---
## Worksheet.SetVisible method

Ställer in de synliga alternativen.

```csharp
public void SetVisible(bool isVisible, bool ignoreError)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isVisible | Boolean | Om kalkylbladet är synligt |
| ignoreError | Boolean | Om fel ska ignoreras om detta alternativ inte är giltigt. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSetVisibleWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några arbetsblad
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Ställ in synlighet för kalkylblad
            // Första parametern: isVisible - false för att dölja bladet
            // Andra parametern: ignoreError - true för att ignorera fel om bladet inte kan döljas
            workbook.Worksheets["Sheet2"].SetVisible(false, true);
            workbook.Worksheets["Sheet3"].SetVisible(false, true);

            // Spara arbetsboken
            workbook.Save("WorksheetVisibilityDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


