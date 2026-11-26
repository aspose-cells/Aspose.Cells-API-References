---
title: "WorkbookSettings.ShowTabs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает значение, указывающее, отображаются ли вкладки Workbook"
type: docs
url: /ru/net/aspose.cells/workbooksettings/showtabs/
---
## WorkbookSettings.ShowTabs property

Получает или задает значение, отображаются ли вкладки книги.

```csharp
public bool ShowTabs { get; set; }
```

### Примечания

Значение по умолчанию — true.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyShowTabsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Скрыть вкладки электронной таблицы
            workbook.Settings.ShowTabs = false;
            
            // Сохраните книгу
            workbook.Save("HideTabsDemo.xlsx", SaveFormat.Xlsx);
            
            // Создать другую книгу для отображения вкладок
            Workbook workbook2 = new Workbook();
            
            // Убедиться, что вкладки видимы (по умолчанию true)
            workbook2.Settings.ShowTabs = true;
            
            // Сохраните книгу
            workbook2.Save("ShowTabsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


