---
title: "Cells.HideRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Скрывает строку"
type: docs
url: /ru/net/aspose.cells/cells/hiderow/
---
## Cells.HideRow method

Скрывает строку.

```csharp
public void HideRow(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Скрыть строку 5
            worksheet.Cells.HideRow(5);
            
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


