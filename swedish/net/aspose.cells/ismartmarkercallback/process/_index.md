---
title: "ISmartMarkerCallBack.Process"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ISmartMarkerCallBack-metod. Återanrop för bearbetning av en smart markör"
type: docs
url: /sv/net/aspose.cells/ismartmarkercallback/process/
---
## ISmartMarkerCallBack.Process method

Återuppringning för bearbetning av en smart marker.

```csharp
public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | Bladindexet. |
| rowIndex | Int32 | Radindexet. |
| colIndex | Int32 | Kolumnindexet. |
| tableName | String | Tabellnamnet för smartmarker. |
| columnName | String | Tabellnamnet för smartmarker. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo : ISmartMarkerCallBack
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo callback = 
                new ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo();

            try
            {
                // Anropa Process-metoden med exempelparametrar
                callback.Process(0, 5, 3, "Products", "ProductName");
                
                Console.WriteLine("Process method executed successfully with parameters (0, 5, 3, \"Products\", \"ProductName\")");
                
                // Ställ in ett värde för att visa effekten
                worksheet.Cells[5, 3].PutValue("ProcessedValue");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
            
            workbook.Save("ISmartMarkerCallBackProcessDemo.xlsx");
        }

        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // Implementering av Process-metoden
            Console.WriteLine($"Processing - Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}, Table: {tableName}, ColumnName: {columnName}");
        }
    }
}
```

### Se även

* interface [ISmartMarkerCallBack](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


