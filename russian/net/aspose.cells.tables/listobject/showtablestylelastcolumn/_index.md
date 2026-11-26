---
title: "ListObject.ShowTableStyleLastColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Указывает, применяется ли стиль к последнему столбцу таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listobject/showtablestylelastcolumn/
---
## ListObject.ShowTableStyleLastColumn property

Указывает, применяется ли стиль к последнему столбцу в таблице.

```csharp
public bool ShowTableStyleLastColumn { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleLastColumnDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Создать объект списка
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];

            // Установить свойство ShowTableStyleLastColumn
            listObject.ShowTableStyleLastColumn = true;

            // Сохраните книгу
            workbook.Save("ListObjectShowLastColumnStyle.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("File saved with ShowTableStyleLastColumn enabled.");
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


