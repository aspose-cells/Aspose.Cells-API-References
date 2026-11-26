---
title: "ListObject.RemoveAutoFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListObject. Удаляет автофильтр, применённый к этой таблице"
type: docs
url: /ru/net/aspose.cells.tables/listobject/removeautofilter/
---
## ListObject.RemoveAutoFilter method

Удаляет автофильтр, примененный к этой таблице.

```csharp
public void RemoveAutoFilter()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodRemoveAutoFilterDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Заполнить примерные данные (с заголовочной строкой)
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Name");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue("Alice");
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue("Bob");
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B4"].PutValue("Charlie");

            try
            {
                // Добавить ListObject (таблицу), который по умолчанию включает автофильтр
                int listIndex = sheet.ListObjects.Add("A1", "B4", true);
                ListObject listObj = sheet.ListObjects[listIndex];

                // Опционально: применить фильтр, чтобы продемонстрировать, что фильтр существует
                listObj.Filter();

                // Удалить автофильтр из ListObject
                listObj.RemoveAutoFilter();

                Console.WriteLine("RemoveAutoFilter called successfully.");
                
                // Сохранить рабочую книгу, чтобы проверить изменения
                workbook.Save("RemoveAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during RemoveAutoFilter operation: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


