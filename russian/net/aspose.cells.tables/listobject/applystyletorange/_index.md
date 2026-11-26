---
title: "ListObject.ApplyStyleToRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListObject. Применить стиль таблицы к диапазону"
type: docs
url: /ru/net/aspose.cells.tables/listobject/applystyletorange/
---
## ListObject.ApplyStyleToRange method

Применить стиль таблицы к диапазону.

```csharp
public void ApplyStyleToRange()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodApplyStyleToRangeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для создания объекта списка
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создать объект списка
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = worksheet.ListObjects[index];

            // Применить стиль к диапазону объекта списка
            listObject.ApplyStyleToRange();

            // Проверить, что стиль применён, проверив цвет переднего плана ячейки
            Style style = worksheet.Cells["A1"].GetStyle();
            Console.WriteLine("Foreground color applied: " + style.ForegroundColor);

            // Преобразовать объект списка в диапазон и проверить
            listObject.ConvertToRange();
            Console.WriteLine("List objects count after conversion: " + worksheet.ListObjects.Count);
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


