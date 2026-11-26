---
title: "Workbook.RemovePersonalInformation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Удаляет личную информацию"
type: docs
url: /ru/net/aspose.cells/workbook/removepersonalinformation/
---
## Workbook.RemovePersonalInformation method

Удаляет личную информацию.

```csharp
public void RemovePersonalInformation()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавить комментарий с информацией об авторе
            int commentIndex = sheet.Comments.Add("A1");
            sheet.Comments[commentIndex].Note = "Sample comment";
            sheet.Comments[commentIndex].Author = "Test Author";
            
            // Отобразить оригинальную информацию об авторе
            Console.WriteLine("Before removal - Comment Author: " + sheet.Comments[commentIndex].Author);
            
            // Удалить личную информацию
            wb.RemovePersonalInformation();
            
            // Сохраните книгу
            wb.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Перезагрузить, чтобы проверить удаление
            Workbook wb2 = new Workbook("output.xlsx");
            Console.WriteLine("After removal - Comment Author: " + wb2.Worksheets[0].Comments[commentIndex].Author);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


