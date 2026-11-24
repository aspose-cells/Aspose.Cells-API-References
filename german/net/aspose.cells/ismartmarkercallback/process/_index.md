---
title: "ISmartMarkerCallBack.Process"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ISmartMarkerCallBack-Methode. Rückruf zur Verarbeitung eines Smart Markers"
type: docs
url: /de/net/aspose.cells/ismartmarkercallback/process/
---
## ISmartMarkerCallBack.Process method

Rückruf für die Verarbeitung eines Smartmarkers.

```csharp
public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | Int32 | Der Blattindex. |
| rowIndex | Int32 | Der Zeilenindex. |
| colIndex | Int32 | Der Spaltenindex. |
| tableName | String | Der Tabellenname des Smartmarkers. |
| columnName | String | Der Tabellenname des Smartmarkers. |

### Beispiele

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
                // Rufen Sie die Process-Methode mit Beispielparametern auf
                callback.Process(0, 5, 3, "Products", "ProductName");
                
                Console.WriteLine("Process method executed successfully with parameters (0, 5, 3, \"Products\", \"ProductName\")");
                
                // Setzen Sie einen Wert, um die Wirkung zu zeigen
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
            // Implementierung der Process-Methode
            Console.WriteLine($"Processing - Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}, Table: {tableName}, ColumnName: {columnName}");
        }
    }
}
```

### Siehe auch

* interface [ISmartMarkerCallBack](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


