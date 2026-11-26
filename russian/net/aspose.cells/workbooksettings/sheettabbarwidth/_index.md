---
title: "WorkbookSettings.SheetTabBarWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Ширина панели вкладок листов в 1/1000 ширины окна"
type: docs
url: /ru/net/aspose.cells/workbooksettings/sheettabbarwidth/
---
## WorkbookSettings.SheetTabBarWidth property

Ширина панели вкладок листа (в 1/1000 ширины окна).

```csharp
public int SheetTabBarWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySheetTabBarWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите свойство SheetTabBarWidth
            workbook.Settings.SheetTabBarWidth = 1000;
            
            // Получите и отобразите значение SheetTabBarWidth
            Console.WriteLine("SheetTabBarWidth: " + workbook.Settings.SheetTabBarWidth);
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


