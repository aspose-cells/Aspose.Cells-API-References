---
title: "WorkbookSettings.FirstVisibleTab"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает первую видимую вкладку листа"
type: docs
url: /ru/net/aspose.cells/workbooksettings/firstvisibletab/
---
## WorkbookSettings.FirstVisibleTab property

Получает или задает первую видимую вкладку листа.

```csharp
public int FirstVisibleTab { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFirstVisibleTabDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить несколько листов
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Установите индекс первой видимой вкладки (нумерация с нуля)
            workbook.Settings.FirstVisibleTab = 1;
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Проверьте настройку
            Console.WriteLine("First visible tab index: " + workbook.Settings.FirstVisibleTab);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


