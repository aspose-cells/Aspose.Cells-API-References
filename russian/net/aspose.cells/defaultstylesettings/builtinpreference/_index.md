---
title: "DefaultStyleSettings.BuiltInPreference"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DefaultStyleSettings. Указывает, предпочтительно ли свойство формата числа, когда стиль определяет как встроенный числовой формат, так и пользовательский шаблон. Значение по умолчанию — false, что означает, что по умолчанию будет использоваться пользовательский шаблон для форматирования значений, если он не пуст для данного стиля"
type: docs
url: /ru/net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

Указывает, предпочтительно ли свойство формата числа, когда стиль определяет как встроенный номер, так и пользовательский шаблон. Значение по умолчанию — false, что означает, что по умолчанию будет использоваться пользовательский шаблон для форматирования значений, если он не пуст для данного стиля.

```csharp
public bool BuiltInPreference { get; set; }
```

### Примечания

При загрузке книги из существующего шаблонного файла могут быть определены как встроенный числовой формат, так и пользовательский шаблон для одного стиля. Это свойство определяет, следует ли использовать встроенный числовой формат или пользовательский шаблон при форматировании значений с этим стилем.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyBuiltInPreferenceDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к настройкам стиля по умолчанию
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Продемонстрировать свойство BuiltInPreference
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12;

            // Применить к worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Сохраните книгу
            workbook.Save("BuiltInPreferenceDemo.xlsx");
        }
    }
}
```

### См. также

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


