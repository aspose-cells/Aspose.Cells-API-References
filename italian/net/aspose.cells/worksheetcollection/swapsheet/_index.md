---
title: "WorksheetCollection.SwapSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorksheetCollection. Scambia i due fogli"
type: docs
url: /it/net/aspose.cells/worksheetcollection/swapsheet/
---
## WorksheetCollection.SwapSheet method

Scambia i due fogli.

```csharp
public void SwapSheet(int sheetIndex1, int sheetIndex2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex1 | Int32 | Il primo foglio di lavoro. |
| sheetIndex2 | Int32 | Il secondo foglio di lavoro. |

### Esempi

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

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


