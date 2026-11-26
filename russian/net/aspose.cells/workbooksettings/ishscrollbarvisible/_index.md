---
title: "WorkbookSettings.IsHScrollBarVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает значение, указывающее, будет ли сгенерированная таблица содержать горизонтальную полосу прокрутки"
type: docs
url: /ru/net/aspose.cells/workbooksettings/ishscrollbarvisible/
---
## WorkbookSettings.IsHScrollBarVisible property

Получает или задает значение, указывающее, будет ли у сгенерированной таблицы горизонтальная полоса прокрутки.

```csharp
public bool IsHScrollBarVisible { get; set; }
```

### Примечания

Значение по умолчанию — true.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;
            
            // Скрыть горизонтальную полосу прокрутки
            settings.IsHScrollBarVisible = false;
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with horizontal scroll bar hidden.");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


