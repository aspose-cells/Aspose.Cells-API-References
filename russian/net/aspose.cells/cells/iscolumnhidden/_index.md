---
title: "Cells.IsColumnHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Проверяет, скрыт ли столбец с заданным индексом"
type: docs
url: /ru/net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

Проверяет, скрыт ли столбец с указанным индексом.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | индекс столбца |

### Возвращаемое значение

true, если столбец скрыт.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsColumnHiddenWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Скрыть столбец C (индекс 2)
            cells.HideColumn(2);
            
            // Проверьте, скрыт ли столбец C
            bool isHidden = cells.IsColumnHidden(2);
            
            Console.WriteLine("Is column C (index 2) hidden? " + isHidden);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


