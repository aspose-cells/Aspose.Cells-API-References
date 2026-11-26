---
title: "Перечисление DisplayDrawingObjects"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.DisplayDrawingObjects enum. Представляет, показывать ли и как показывать объекты в рабочей книге"
type: docs
url: /ru/net/aspose.cells/displaydrawingobjects/
---
## DisplayDrawingObjects enumeration

Представляет, показывать ли и как отображать объекты в рабочей книге.

```csharp
public enum DisplayDrawingObjects
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DisplayShapes | `0` | Показать все объекты |
| Placeholders | `1` | Показать заполнители |
| Hide | `2` | Скрыть все фигуры. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DisplayDrawingObjectsDemo
    {
        public static void DisplayDrawingObjectsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к настройкам книги
            WorkbookSettings settings = workbook.Settings;

            // Установите свойство DisplayDrawingObjects, чтобы показать все объекты
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;

            // Сохраните книгу
            workbook.Save("DisplayDrawingObjectsExample_DisplayShapes.xlsx");

            // Установите свойство DisplayDrawingObjects, чтобы показать заполнители
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;

            // Сохраните книгу
            workbook.Save("DisplayDrawingObjectsExample_Placeholders.xlsx");

            // Установите свойство DisplayDrawingObjects, чтобы скрыть все фигуры
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;

            // Сохраните книгу
            workbook.Save("DisplayDrawingObjectsExample_Hide.xlsx");
            workbook.Save("DisplayDrawingObjectsExample_Hide.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


