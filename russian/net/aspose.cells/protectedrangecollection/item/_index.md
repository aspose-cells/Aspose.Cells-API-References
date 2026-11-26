---
title: "ProtectedRangeCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ProtectedRangeCollection. Возвращает элемент ProtectedRange по указанному индексу"
type: docs
url: /ru/net/aspose.cells/protectedrangecollection/item/
---
## ProtectedRangeCollection indexer

Возвращает элемент [`ProtectedRange`](../../protectedrange/) по указанному индексу.

```csharp
public ProtectedRange this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте защищённый диапазон, используя индексы ячеек (startRow, startColumn, endRow, endColumn)
            int index = worksheet.AllowEditRanges.Add("MyProtectedRange", 0, 0, 1, 1);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[index];
            protectedRange.Password = "password123";
            
            // Получите доступ к защищённому диапазону, используя свойство Item (index 0)
            ProtectedRange retrievedRange = worksheet.AllowEditRanges[0];
            
            // Проверьте и отобразите статус защиты
            Console.WriteLine("Is protected with password: " + retrievedRange.IsProtectedWithPassword);
            Console.WriteLine("Range name: " + retrievedRange.Name);
            
            // Сохраните книгу
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [ProtectedRange](../../protectedrange/)
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


