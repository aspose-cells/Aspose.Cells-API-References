---
title: "Cells.MinDataRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Минимальный индекс строки ячейки, содержащей данные"
type: docs
url: /ru/net/aspose.cells/cells/mindatarow/
---
## Cells.MinDataRow property

Минимальный индекс строки ячейки, содержащей данные.

```csharp
public int MinDataRow { get; }
```

### Примечания

Возвращает -1, если нет ячейки, содержащей данные. Это свойство требует итерации и динамической проверки ячеек и строк, поэтому является ресурсоёмким процессом и не должно вызываться многократно, например, использовать его напрямую в условии цикла.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataRowDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Заполните некоторыми данными
            sheet.Cells[0, 0].Value = "Header1";
            sheet.Cells[0, 1].Value = "Header2";
            sheet.Cells[1, 0].Value = "Data1";
            sheet.Cells[1, 1].Value = "Data2";
            sheet.Cells[2, 0].Value = "Data3";
            sheet.Cells[2, 1].Value = "Data4";

            // Продемонстрировать использование MinDataRow
            Console.WriteLine("Minimum data row index: " + sheet.Cells.MinDataRow);
            Console.WriteLine("Maximum data row index: " + sheet.Cells.MaxDataRow);

            // Сохраните книгу
            workbook.Save("MinDataRowExample.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


