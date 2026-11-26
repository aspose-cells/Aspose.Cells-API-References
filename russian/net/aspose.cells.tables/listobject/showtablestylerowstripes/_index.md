---
title: "ListObject.ShowTableStyleRowStripes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Указывает, применяется ли форматирование полос строк к"
type: docs
url: /ru/net/aspose.cells.tables/listobject/showtablestylerowstripes/
---
## ListObject.ShowTableStyleRowStripes property

Указывает, применяется ли форматирование полос строк к.

```csharp
public bool ShowTableStyleRowStripes { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleRowStripesDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);

            // Создать объект списка
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];

            // Продемонстрировать свойство ShowTableStyleRowStripes
            Console.WriteLine("Before: ShowTableStyleRowStripes = " + listObject.ShowTableStyleRowStripes);
            listObject.ShowTableStyleRowStripes = false;
            Console.WriteLine("After: ShowTableStyleRowStripes = " + listObject.ShowTableStyleRowStripes);

            // Сохраните книгу
            workbook.Save("ListObjectShowTableStyleRowStripesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


