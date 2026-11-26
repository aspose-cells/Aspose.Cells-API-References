---
title: "Cell.InsertText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Вставить несколько символов в ячейку. Если ячейка имеет богатое форматирование, этот метод может сохранить исходное форматирование"
type: docs
url: /ru/net/aspose.cells/cell/inserttext/
---
## Cell.InsertText method

Вставляет несколько символов в ячейку. Если ячейка имеет богатое форматирование, этот метод может сохранить исходное форматирование.

```csharp
public void InsertText(int index, string text)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс. |
| текст | String | Вставленный текст. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите доступ к ячейке B3 и задайте начальное значение
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("OriginalText");
            
            // Вставьте текст в позицию 6
            cell.InsertText(6, "Inserted");
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


