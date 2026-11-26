---
title: "WorksheetCollection.GetNamedRangesAndTables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Получает все предопределённые именованные диапазоны в таблице"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/getnamedrangesandtables/
---
## WorksheetCollection.GetNamedRangesAndTables method

Получает все предопределённые именованные диапазоны в электронной таблице.

```csharp
public Range[] GetNamedRangesAndTables()
```

### Возвращаемое значение

Массив объектов Range.

Возвращает null, если именованный диапазон не существует.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetNamedRangesAndTablesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать несколько именованных диапазонов
            worksheet.Cells.CreateRange("A1:B2").Name = "TestRange1";
            worksheet.Cells.CreateRange("C3:D4").Name = "TestRange2";
            
            // Получить все именованные диапазоны и таблицы
            Aspose.Cells.Range[] ranges = workbook.Worksheets.GetNamedRangesAndTables();
            
            // Отобразить информацию о диапазонах
            Console.WriteLine("Found {0} named ranges:", ranges.Length);
            foreach (Aspose.Cells.Range range in ranges)
            {
                Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
            }
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


