---
title: "WorksheetCollection.SwapSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Byter plats på de två bladen"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/swapsheet/
---
## WorksheetCollection.SwapSheet method

Byter plats på de två bladen.

```csharp
public void SwapSheet(int sheetIndex1, int sheetIndex2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex1 | Int32 | Det första kalkylbladet. |
| sheetIndex2 | Int32 | Det andra kalkylbladet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSwapSheetWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets[0].Name = "Sheet1";
            workbook.Worksheets[1].Name = "Sheet2";
            
            workbook.Worksheets[0].Cells["A1"].PutValue("FirstSheet");
            workbook.Worksheets[1].Cells["A1"].PutValue("SecondSheet");
            
            Console.WriteLine("Before swap:");
            Console.WriteLine("Sheet1 A1: " + workbook.Worksheets[0].Cells["A1"].StringValue);
            Console.WriteLine("Sheet2 A1: " + workbook.Worksheets[1].Cells["A1"].StringValue);
            
            workbook.Worksheets.SwapSheet(0, 1);
            
            Console.WriteLine("\nAfter swap:");
            Console.WriteLine("Sheet1 A1: " + workbook.Worksheets[0].Cells["A1"].StringValue);
            Console.WriteLine("Sheet2 A1: " + workbook.Worksheets[1].Cells["A1"].StringValue);
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


