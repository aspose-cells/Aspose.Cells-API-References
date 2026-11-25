---
title: "ISmartMarkerCallBack.Process"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ISmartMarkerCallBack. Callback per l'elaborazione di un smart marker"
type: docs
url: /it/net/aspose.cells/ismartmarkercallback/process/
---
## ISmartMarkerCallBack.Process method

Callback per l'elaborazione di un smart marker.

```csharp
public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | Int32 | L'indice del foglio. |
| rowIndex | Int32 | L'indice della riga. |
| colIndex | Int32 | L'indice della colonna. |
| tableName | String | Il nome della tabella dello smartmarker. |
| columnName | String | Il nome della tabella dello smartmarker. |

### Esempi

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
                // Chiama il metodo Process con parametri di esempio
                callback.Process(0, 5, 3, "Products", "ProductName");
                
                Console.WriteLine("Process method executed successfully with parameters (0, 5, 3, \"Products\", \"ProductName\")");
                
                // Imposta un valore per mostrare l'effetto
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
            // Implementazione del metodo Process
            Console.WriteLine($"Processing - Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}, Table: {tableName}, ColumnName: {columnName}");
        }
    }
}
```

### Vedi anche

* interface [ISmartMarkerCallBack](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


