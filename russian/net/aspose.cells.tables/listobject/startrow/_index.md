---
title: "ListObject.StartRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Возвращает начальную строку диапазона"
type: docs
url: /ru/net/aspose.cells.tables/listobject/startrow/
---
## ListObject.StartRow property

Получает начальную строку диапазона.

```csharp
public int StartRow { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyStartRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать образцовые данные, начиная со строки 2
            worksheet.Cells["A2"].PutValue("ID");
            worksheet.Cells["B2"].PutValue("Name");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue("John");
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["B4"].PutValue("Mary");

            // Создать объект списка, начиная со строки 2
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Отобразить свойство StartRow
            Console.WriteLine("ListObject StartRow: " + listObject.StartRow);

            // Чтобы "изменить" начальную строку, нам нужно воссоздать ListObject
            worksheet.ListObjects.RemoveAt(listObjectIndex);
            listObjectIndex = worksheet.ListObjects.Add(2, 0, 3, 1, true);
            listObject = worksheet.ListObjects[listObjectIndex];
            
            Console.WriteLine("Modified ListObject StartRow: " + listObject.StartRow);
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


