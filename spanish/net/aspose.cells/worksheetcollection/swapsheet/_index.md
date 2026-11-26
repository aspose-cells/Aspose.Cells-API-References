---
title: "WorksheetCollection.SwapSheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Intercambia las dos hojas"
type: docs
url: /es/net/aspose.cells/worksheetcollection/swapsheet/
---
## WorksheetCollection.SwapSheet method

Intercambia las dos hojas.

```csharp
public void SwapSheet(int sheetIndex1, int sheetIndex2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex1 | Int32 | La primera hoja de cálculo. |
| sheetIndex2 | Int32 | La segunda hoja de cálculo. |

### Ejemplos

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

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


