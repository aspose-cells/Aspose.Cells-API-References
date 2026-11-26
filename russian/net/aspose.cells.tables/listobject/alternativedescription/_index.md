---
title: "ListObject.AlternativeDescription"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Получает и задает альтернативное описание"
type: docs
url: /ru/net/aspose.cells.tables/listobject/alternativedescription/
---
## ListObject.AlternativeDescription property

Получает и задает альтернативное описание.

```csharp
public string AlternativeDescription { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeDescriptionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создать объект списка
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Установить альтернативный текст и описание
            listObject.AlternativeText = "Test";
            listObject.AlternativeDescription = "aSXADCS";

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Перезагрузите и проверьте свойства
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedListObject = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedListObject.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedListObject.AlternativeDescription);
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


