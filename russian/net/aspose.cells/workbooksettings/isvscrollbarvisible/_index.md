---
title: "WorkbookSettings.IsVScrollBarVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает значение, указывающее, будет ли в сгенерированной таблице вертикальная полоса прокрутки"
type: docs
url: /ru/net/aspose.cells/workbooksettings/isvscrollbarvisible/
---
## WorkbookSettings.IsVScrollBarVisible property

Получает или задает значение, указывающее, будет ли сгенерированная таблица содержать вертикальную полосу прокрутки.

```csharp
public bool IsVScrollBarVisible { get; set; }
```

### Примечания

Значение по умолчанию — true.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsVScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;
            
            // Скройте вертикальную полосу прокрутки
            settings.IsVScrollBarVisible = false;
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Vertical scroll bar visibility set to false. Workbook saved.");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


