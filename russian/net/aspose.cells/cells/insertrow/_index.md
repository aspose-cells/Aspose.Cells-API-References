---
title: "Cells.InsertRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Вставляет новую строку в лист"
type: docs
url: /ru/net/aspose.cells/cells/insertrow/
---
## Cells.InsertRow method

Вставляет новую строку в лист.

```csharp
public void InsertRow(int rowIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Получить коллекцию ячеек
            Cells cells = sheet.Cells;
            
            // Вставьте примерные данные в строку 6
            cells[6, 0].PutValue("Original Row 6");
            cells[6, 1].PutValue(100);
            
            // Вставьте примерные данные в строку 7
            cells[7, 0].PutValue("Original Row 7");
            cells[7, 1].PutValue(200);
            
            // Вставьте новую строку по индексу 7 (сдвигает существующую строку 7 вниз)
            cells.InsertRow(7);
            
            // Добавьте данные в только что вставленную строку
            cells[7, 0].PutValue("New Inserted Row");
            cells[7, 1].PutValue(150);
            
            // Сохраните книгу
            workbook.Save("InsertRowDemo.xlsx");
            
            Console.WriteLine("Row inserted successfully at index 7.");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


