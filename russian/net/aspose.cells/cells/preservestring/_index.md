---
title: "Cells.PreserveString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает или задает значение, указывающее, сохраняются ли все значения листа как строки. По умолчанию false"
type: docs
url: /ru/net/aspose.cells/cells/preservestring/
---
## Cells.PreserveString property

Получает или задает значение, указывающее, сохраняются ли все значения листа как строки. По умолчанию — false.

```csharp
public bool PreserveString { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyPreserveStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить свойство PreserveString в true
            cells.PreserveString = true;

            // Добавить строковые значения в ячейки
            cells["A1"].PutValue("Preserved String 1");
            cells["B1"].PutValue("Preserved String 2");

            // Получить доступ к значениям (они будут сохранены как строки)
            Console.WriteLine("Cell A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + cells["B1"].StringValue);

            // Сохраните книгу
            workbook.Save("PreserveStringDemo.xlsx", SaveFormat.Xlsx);

            // Загрузить сохранённую книгу, чтобы проверить сохранение
            Workbook loadedWorkbook = new Workbook("PreserveStringDemo.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;

            // Вывести сохранённые значения
            Console.WriteLine("\nAfter loading:");
            Console.WriteLine("Cell A1 value: " + loadedCells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + loadedCells["B1"].StringValue);

            // Продемонстрировать сравнение свойства PreserveString
            Console.WriteLine("\nPreserveString property matches: " + 
                (cells.PreserveString == loadedCells.PreserveString));
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


