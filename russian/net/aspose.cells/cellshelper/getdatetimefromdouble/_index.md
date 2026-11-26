---
title: "CellsHelper.GetDateTimeFromDouble"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Преобразует значение double в значение даты и времени"
type: docs
url: /ru/net/aspose.cells/cellshelper/getdatetimefromdouble/
---
## CellsHelper.GetDateTimeFromDouble method

Преобразует значение double в значение даты и времени.

```csharp
public static DateTime GetDateTimeFromDouble(double doubleValue, bool date1904)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| doubleValue | Double | Значение double. |
| date1904 | Boolean | Система даты 1904. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetDateTimeFromDoubleWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте данные для параметров метода (Double, Boolean)
            double doubleValue = 44197.5; // Represents 2021-01-01 12:00:00 in Excel serial date format
            bool date1904 = false; // Using 1900 date system

            try
            {
                // Вызовите метод GetDateTimeFromDouble с конкретными типами параметров
                DateTime result = CellsHelper.GetDateTimeFromDouble(doubleValue, date1904);
                
                // Отобразить результат
                Console.WriteLine($"Converted DateTime: {result}");
                
                // Запишите результат в ячейку
                worksheet.Cells["A1"].PutValue("Original Double Value:");
                worksheet.Cells["B1"].PutValue(doubleValue);
                worksheet.Cells["A2"].PutValue("Converted DateTime:");
                worksheet.Cells["B2"].PutValue(result.ToString());
                
                Console.WriteLine("Method executed successfully with parameters (Double, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDateTimeFromDouble method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("MethodGetDateTimeFromDoubleDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


