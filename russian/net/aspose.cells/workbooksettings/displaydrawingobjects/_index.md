---
title: "WorkbookSettings.DisplayDrawingObjects"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает, показывать ли объекты в книге и как это делать"
type: docs
url: /ru/net/aspose.cells/workbooksettings/displaydrawingobjects/
---
## WorkbookSettings.DisplayDrawingObjects property

Указывает, показывать ли объекты в рабочей книге и как их отображать.

```csharp
public DisplayDrawingObjects DisplayDrawingObjects { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDisplayDrawingObjectsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к настройкам книги
            WorkbookSettings settings = workbook.Settings;

            // Добавьте образец фигуры, чтобы продемонстрировать свойство
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Установить отображение всех фигур
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
            workbook.Save("DisplayShapes.xlsx");

            // Установить отображение заполнителей
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;
            workbook.Save("Placeholders.xlsx");

            // Установить скрытие всех фигур
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;
            workbook.Save("Hide.xlsx");
        }
    }
}
```

### См. также

* enum [DisplayDrawingObjects](../../displaydrawingobjects/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


