---
title: "WorkbookSettings.SetPageOrientationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorkbookSettings. Устанавливает тип ориентации печати для всей книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/setpageorientationtype/
---
## WorkbookSettings.SetPageOrientationType method

Устанавливает тип ориентации печати для всей книги.

```csharp
public void SetPageOrientationType(PageOrientationType pageOrientationType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageOrientationType | PageOrientationType | Тип ориентации страницы |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodSetPageOrientationTypeWithPageOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            
            // Установить ориентацию страницы в Portrait для всех листов
            workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
            
            // Проверьте, что ориентация установлена правильно
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine("Worksheet: " + sheet.Name + " - Orientation: " + sheet.PageSetup.Orientation);
            }
        }
    }
}
```

### См. также

* enum [PageOrientationType](../../pageorientationtype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


