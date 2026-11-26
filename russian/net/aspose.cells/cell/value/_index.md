---
title: "Cell.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получает/устанавливает значение, содержащееся в этой ячейке"
type: docs
url: /ru/net/aspose.cells/cell/value/
---
## Cell.Value property

Получает/устанавливает значение, содержащееся в этой ячейке.

```csharp
public object Value { get; set; }
```

### Примечания

Возможный тип:

null,

Boolean,

DateTime,

Double,

Integer

String.

Для значения типа int оно может быть возвращено как объект Integer, либо как объект Double. И нет гарантии, что возвращаемое значение всегда будет сохранено как объект того же типа.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите значения, используя свойство Value
            cells[0, 0].Value = "Product ID";
            cells[0, 1].Value = "Product Name";
            
            // Продемонстрировать null‑значения
            cells[0, 2].Value = null;
            cells[1, 0].Value = null;
            cells[1, 1].Value = null;
            cells[1, 2].Value = null;

            // Отобразить значения
            Console.WriteLine("Cell[0,0] Value: " + cells[0, 0].Value);
            Console.WriteLine("Cell[0,1] Value: " + cells[0, 1].Value);
            Console.WriteLine("Cell[0,2] Value: " + (cells[0, 2].Value == null ? "null" : cells[0, 2].Value));
            Console.WriteLine("Cell[1,0] Value: " + (cells[1, 0].Value == null ? "null" : cells[1, 0].Value));
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


