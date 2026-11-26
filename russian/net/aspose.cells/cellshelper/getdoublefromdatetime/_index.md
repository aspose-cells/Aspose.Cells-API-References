---
title: "CellsHelper.GetDoubleFromDateTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Преобразовать дату и время в значение типа double"
type: docs
url: /ru/net/aspose.cells/cellshelper/getdoublefromdatetime/
---
## CellsHelper.GetDoubleFromDateTime method

Преобразует дату и время в значение double.

```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dateTime | DateTime | Дата и время. |
| date1904 | Boolean | Система даты 1904. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetDoubleFromDateTimeWithDateTimeBooleanDemo
    {
        public static void Run()
        {
            // Создать экземпляр рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить текущие дату и время
            DateTime now = DateTime.Now;
            
            // Преобразовать DateTime в double с помощью CellsHelper
            double dateDouble = CellsHelper.GetDoubleFromDateTime(now, false);
            
            // Установить значение в ячейку A1
            worksheet.Cells["A1"].PutValue(dateDouble);
            
            // Форматировать ячейку для отображения как дата
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Number = 14; // Date format
            worksheet.Cells["A1"].SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("DateTimeConversionDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


