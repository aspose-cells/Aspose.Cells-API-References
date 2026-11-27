---
title: "Worksheet.MoveTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Flyttar bladet till en annan plats i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/moveto/
---
## Worksheet.MoveTo method

Flyttar bladet till en annan plats i kalkylbladet.

```csharp
public void MoveTo(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Destinationsbladets index. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodMoveToWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några arbetsblad
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Lägg till ett nytt arbetsblad och flytta det till position 1
            Worksheet newWorksheet = workbook.Worksheets.Add("MovedSheet");
            newWorksheet.MoveTo(1);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


