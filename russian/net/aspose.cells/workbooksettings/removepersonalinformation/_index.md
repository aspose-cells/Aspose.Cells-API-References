---
title: "WorkbookSettings.RemovePersonalInformation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Истина, если личная информация может быть удалена из указанной книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/removepersonalinformation/
---
## WorkbookSettings.RemovePersonalInformation property

Истина, если из указанной книги можно удалить персональные данные.

```csharp
public bool RemovePersonalInformation { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить RemovePersonalInformation в значение true
            workbook.Settings.RemovePersonalInformation = true;
            
            // Добавьте некоторые образцы данных.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Email");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue("john@example.com");
            
            // Сохраните книгу
            string outputPath = "output_with_personal_info_removed.xlsx";
            workbook.Save(outputPath);
            
            // Загрузите сохранённую книгу, чтобы проверить настройку
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("RemovePersonalInformation setting: " + 
                loadedWorkbook.Settings.RemovePersonalInformation);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


