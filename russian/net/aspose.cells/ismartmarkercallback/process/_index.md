---
title: "ISmartMarkerCallBack.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ISmartMarkerCallBack. Обратный вызов для обработки смарт‑маркера"
type: docs
url: /ru/net/aspose.cells/ismartmarkercallback/process/
---
## ISmartMarkerCallBack.Process method

Обратный вызов для обработки смарт‑маркера.

```csharp
public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | Индекс листа. |
| rowIndex | Int32 | Индекс строки. |
| colIndex | Int32 | Индекс столбца. |
| tableName | String | Имя таблицы смарт‑маркера. |
| columnName | String | Имя таблицы смарт‑маркера. |

### Примеры

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
                // Вызвать метод Process с примерными параметрами
                callback.Process(0, 5, 3, "Products", "ProductName");
                
                Console.WriteLine("Process method executed successfully with parameters (0, 5, 3, \"Products\", \"ProductName\")");
                
                // Установить значение, чтобы показать эффект
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
            // Реализация метода Process
            Console.WriteLine($"Processing - Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}, Table: {tableName}, ColumnName: {columnName}");
        }
    }
}
```

### См. также

* interface [ISmartMarkerCallBack](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


