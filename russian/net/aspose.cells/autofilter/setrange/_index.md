---
title: "AutoFilter.SetRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Устанавливает диапазон, к которому применяется указанный AutoFilter"
type: docs
url: /ru/net/aspose.cells/autofilter/setrange/
---
## AutoFilter.SetRange method

Устанавливает диапазон, к которому применяется указанный AutoFilter.

```csharp
public void SetRange(int row, int startColumn, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| startColumn | Int32 | Индекс начального столбца. |
| endColumn | Int32 | Индекс конечного столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodSetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A4"].PutValue("Data3");

            // Установить диапазон автофильтра (firstRow, firstColumn, totalRows)
            sheet.AutoFilter.SetRange(0, 0, 4);

            // Применить фильтр
            sheet.AutoFilter.Custom(0, FilterOperatorType.Equal, "Data2");

            // Обновить фильтр
            sheet.AutoFilter.Refresh();

            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


