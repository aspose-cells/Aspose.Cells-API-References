---
title: "Класс DefaultStyleSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DefaultStyleSettings. Настройки значений по умолчанию свойств стилей книги"
type: docs
url: /ru/net/aspose.cells/defaultstylesettings/
---
## DefaultStyleSettings class

Настройки значений по умолчанию свойств стилей книги.

```csharp
public class DefaultStyleSettings
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BuiltInPreference](../../aspose.cells/defaultstylesettings/builtinpreference/) { get; set; } | Указывает, предпочтительно ли свойство формата числа, когда стиль определяет как встроенный номер, так и пользовательский шаблон. Значение по умолчанию — false, что означает, что по умолчанию будет использоваться пользовательский шаблон для форматирования значений, если он не пуст для данного стиля. |
| [FontName](../../aspose.cells/defaultstylesettings/fontname/) { get; set; } | Получает/Устанавливает имя шрифта по умолчанию для книги |
| [FontSize](../../aspose.cells/defaultstylesettings/fontsize/) { get; set; } | Получает/Устанавливает стандартный размер шрифта по умолчанию для книги. |
| [HorizontalAlignment](../../aspose.cells/defaultstylesettings/horizontalalignment/) { get; set; } | Получает/Устанавливает значение по умолчанию для горизонтального выравнивания |
| [VerticalAlignment](../../aspose.cells/defaultstylesettings/verticalalignment/) { get; set; } | Получает/Устанавливает значение по умолчанию для вертикального выравнивания |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultStyleSettingsDemo
    {
        public static void DefaultStyleSettingsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к настройкам стиля по умолчанию книги
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Установка свойств
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12.0;
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
            defaultStyleSettings.VerticalAlignment = TextAlignmentType.Center;

            // Примените настройки стиля по умолчанию к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            // Сохраните книгу
            workbook.Save("DefaultStyleSettingsExample.xlsx");
            workbook.Save("DefaultStyleSettingsExample.pdf");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


