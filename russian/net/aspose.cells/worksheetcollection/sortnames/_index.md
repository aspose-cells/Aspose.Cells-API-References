---
title: "WorksheetCollection.SortNames"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorksheetCollection метод. Сортирует определённые имена"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/sortnames/
---
## WorksheetCollection.SortNames method

Сортирует определённые имена.

```csharp
public void SortNames()
```

### Примечания

Если вы создаёте большое количество именованных диапазонов в файле Excel, пожалуйста, вызовите этот метод после создания всех именованных диапазонов и перед сохранением.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSortNamesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить несколько именованных диапазонов
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test1");
            worksheet.Cells.CreateRange("A1").Name = "Range2";
            worksheet.Cells["B1"].PutValue("Test2");
            worksheet.Cells.CreateRange("B1").Name = "Range1";
            
            // Отобразить имена до сортировки
            Console.WriteLine("Before sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Отсортировать имена
            workbook.Worksheets.SortNames();
            
            // Отобразить имена после сортировки
            Console.WriteLine("\nAfter sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


