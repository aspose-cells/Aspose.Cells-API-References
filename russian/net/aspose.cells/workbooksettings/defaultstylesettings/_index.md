---
title: "WorkbookSettings.DefaultStyleSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает настройки значений по умолчанию для свойств, связанных со стилем, этой книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/defaultstylesettings/
---
## WorkbookSettings.DefaultStyleSettings property

Получает настройки значений по умолчанию свойств, связанных со стилем, для этой рабочей книги.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к настройкам стиля по умолчанию
            DefaultStyleSettings styleSettings = workbook.Settings.DefaultStyleSettings;

            // Установить предпочтение встроенного числового формата
            styleSettings.BuiltInPreference = true;

            // Установить культуру для форматирования чисел
            workbook.Settings.CultureInfo = new CultureInfo("en-US");

            // Получить доступ к ячейкам и применить форматирование
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите значения и стили
            cells["A1"].PutValue(1234.56);
            cells["A1"].GetStyle().Number = 4; // Currency format

            cells["B1"].PutValue(0.456);
            cells["B1"].GetStyle().Number = 2; // Percentage format

            cells["C1"].PutValue(DateTime.Now);
            cells["C1"].GetStyle().Number = 22; // Short date format

            // Сохраните книгу
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
        }
    }
}
```

### См. также

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


