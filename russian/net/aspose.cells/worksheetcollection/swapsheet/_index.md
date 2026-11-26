---
title: "WorksheetCollection.SwapSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Меняет местами два листа"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/swapsheet/
---
## WorksheetCollection.SwapSheet method

Меняет местами два листа.

```csharp
public void SwapSheet(int sheetIndex1, int sheetIndex2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex1 | Int32 | Первый рабочий лист. |
| sheetIndex2 | Int32 | Второй рабочий лист. |

### Примеры

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

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


