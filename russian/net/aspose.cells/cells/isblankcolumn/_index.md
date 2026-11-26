---
title: "Cells.IsBlankColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Проверяет, является ли указанный столбец пустым, не содержит ли данных"
type: docs
url: /ru/net/aspose.cells/cells/isblankcolumn/
---
## Cells.IsBlankColumn method

Проверяет, является ли указанный столбец пустым (не содержит данных).

```csharp
public bool IsBlankColumn(int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | индекс столбца |

### Возвращаемое значение

true, если указанный столбец не содержит данных

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsBlankColumnWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Проверьте, пустой ли столбец 2 (должно быть true для нового листа)
            Console.WriteLine("Is column 2 blank? " + worksheet.Cells.IsBlankColumn(1));

            // Добавьте данные в столбец 2
            worksheet.Cells["B1"].PutValue("Test Data");

            // Проверьте снова (теперь должно быть false)
            Console.WriteLine("Is column 2 blank after adding data? " + worksheet.Cells.IsBlankColumn(1));

            // Создайте другой лист с полностью пустыми столбцами
            Worksheet worksheet2 = workbook.Worksheets.Add("BlankSheet");

            // Проверьте столбец в пустом листе (должно быть true)
            Console.WriteLine("Is column 3 blank in new sheet? " + worksheet2.Cells.IsBlankColumn(2));
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


