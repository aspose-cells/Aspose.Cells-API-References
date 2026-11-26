---
title: "Cells.UnhideRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Отображает скрытую строку"
type: docs
url: /ru/net/aspose.cells/cells/unhiderow/
---
## Cells.UnhideRow method

Отображает скрытую строку.

```csharp
public void UnhideRow(int row, double height)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| высота | Double | Высота строки. Высота строки будет изменена только когда строка скрыта и заданное значение высоты положительно. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Скрыть строку 5
            worksheet.Cells.HideRow(5);
            
            // Отобразить строку 5 с высотой 12.75
            worksheet.Cells.UnhideRow(5, 12.75);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


