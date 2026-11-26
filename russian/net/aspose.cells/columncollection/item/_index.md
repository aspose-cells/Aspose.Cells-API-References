---
title: "ColumnCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ColumnCollection. Возвращает объект Column по индексу столбца. Объект Column с указанным индексом будет создан, если он ранее не существовал"
type: docs
url: /ru/net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

Возвращает объект [`Column`](../../column/) по индексу столбца. Объект Column с указанным индексом будет создан, если он ранее не существовал.

```csharp
public Column this[int columnIndex] { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите доступ к коллекции столбцов
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Установите ширину столбцов с помощью свойства Item
            columns[0].Width = 10;
            columns[1].Width = 15;
            columns[2].Width = 20;
            
            // Отобразите ширины столбцов
            Console.WriteLine("Column 0 Width: " + columns[0].Width);
            Console.WriteLine("Column 1 Width: " + columns[1].Width);
            Console.WriteLine("Column 2 Width: " + columns[2].Width);
            
            // Проверьте, что ширины столбцов установлены правильно
            if (columns[0].Width != 10 || columns[1].Width != 15 || columns[2].Width != 20)
            {
                throw new Exception("Column widths were not set correctly");
            }
        }
    }
}
```

### См. также

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


