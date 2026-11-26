---
title: "ListObject.ShowTableStyleFirstColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Указывает, применяется ли стиль к первому столбцу таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listobject/showtablestylefirstcolumn/
---
## ListObject.ShowTableStyleFirstColumn property

Указывает, применяется ли стиль к первому столбцу в таблице.

```csharp
public bool ShowTableStyleFirstColumn { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleFirstColumnDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["B4"].PutValue(3.2);

            // Создать объект списка
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];
            
            // Применить стиль первого столбца
            listObject.ShowTableStyleFirstColumn = true;
            
            // Сохраните книгу
            workbook.Save("ListObjectShowFirstColumnStyle.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("File saved with first column style applied to the table.");
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


