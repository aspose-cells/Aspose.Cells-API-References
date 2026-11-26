---
title: "WorkbookSettings.Password"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Представляет пароль шифрования файла книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/password/
---
## WorkbookSettings.Password property

Представляет пароль шифрования файла Workbook.

```csharp
public string Password { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получить доступ к первому листу и добавить данные
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["C6"].PutValue("test encrypt.");
            
            // Установите пароль для защиты книги
            wb.Settings.Password = "xixi";
            
            // Сохраните книгу
            wb.Save("output_with_password.ods");
            
            // Создайте параметры загрузки с паролем, чтобы открыть защищённую книгу
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "xixi";
            
            // Откройте книгу, защищённую паролем
            Workbook wbProtected = new Workbook("output_with_password.ods", loadOptions);
            
            // Проверьте данные
            Console.WriteLine("Cell value: " + wbProtected.Worksheets[0].Cells["C6"].Value);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


