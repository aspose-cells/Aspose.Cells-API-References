---
title: "LoadOptions.DefaultStyleSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Получает настройки стиля по умолчанию для инициализации стилей рабочей книги"
type: docs
url: /ru/net/aspose.cells/loadoptions/defaultstylesettings/
---
## LoadOptions.DefaultStyleSettings property

Получает параметры стиля по умолчанию для инициализации стилей рабочей книги

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите параметры загрузки с настройками стиля по умолчанию
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
            
            // Создайте лист и получите ячейки
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Установите значения для демонстрации стиля по умолчанию
            cells["A1"].PutValue("Default Style Applied");
            cells["A2"].PutValue("Should have bottom alignment");
            
            // Создайте ячейку с пользовательским стилем (для сравнения с по умолчанию)
            Cell customCell = cells["B1"];
            customCell.PutValue("Custom Style");
            Style customStyle = customCell.GetStyle();
            customStyle.VerticalAlignment = TextAlignmentType.Center;
            customCell.SetStyle(customStyle);
            
            // Сохраните книгу
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
            
            // Проверьте стили
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("B1 Vertical Alignment: " + cells["B1"].GetStyle().VerticalAlignment);
        }
    }
}
```

### См. также

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


