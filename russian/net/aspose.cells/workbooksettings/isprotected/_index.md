---
title: "WorkbookSettings.IsProtected"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorkbookSettings property. Возвращает значение, указывающее, защищена ли структура или окно рабочей книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/isprotected/
---
## WorkbookSettings.IsProtected property

Получает значение, указывающее, защищены ли структура или окно рабочей книги.

```csharp
public bool IsProtected { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;
            
            // Проверьте, защищена ли рабочая книга
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Защитить книгу паролем
            settings.Password = "password123";
            
            // Проверить статус защиты
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Сохранить защищённую книгу
            workbook.Save("ProtectedWorkbook.xlsx", SaveFormat.Xlsx);
            
            // Откройте защищённую рабочую книгу
            Workbook protectedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            
            // Проверьте статус защиты загруженной рабочей книги
            Console.WriteLine("Loaded workbook is protected: " + protectedWorkbook.Settings.IsProtected);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


