---
title: "Cells.TextToColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Разделяет содержимое указанного столбца на несколько столбцов"
type: docs
url: /ru/net/aspose.cells/cells/texttocolumns/
---
## Cells.TextToColumns method

Разделяет содержимое указанного столбца на несколько столбцов..

```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |
| totalRows | Int32 | Количество строк. |
| опции | TxtLoadOptions | Параметры разделения. |

### Возвращаемое значение

Общее количество столбцов разделённых значений.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodTextToColumnsWithInt32Int32Int32TxtLoadOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Установите примерные данные со значениями, разделёнными запятыми
            sheet.Cells["A1"].PutValue("John,Doe,30");
            sheet.Cells["A2"].PutValue("Jane,Smith,28");

            // Создайте параметры загрузки текста, используя запятую в качестве разделителя
            TxtLoadOptions options = new TxtLoadOptions();
            options.Separator = ',';

            // Разделите текст по столбцам, начиная с ячейки A1, шириной в 3 столбца
            sheet.Cells.TextToColumns(0, 0, 3, options);

            // Проверьте результаты
            Console.WriteLine("B1: " + sheet.Cells["B1"].StringValue); // Should output "Doe"
            Console.WriteLine("C2: " + sheet.Cells["C2"].StringValue); // Should output "28"

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


