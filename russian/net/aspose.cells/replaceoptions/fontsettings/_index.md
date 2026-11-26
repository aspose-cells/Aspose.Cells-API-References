---
title: "ReplaceOptions.FontSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReplaceOptions. Форматированные настройки для заменяемого текста"
type: docs
url: /ru/net/aspose.cells/replaceoptions/fontsettings/
---
## ReplaceOptions.FontSettings property

Настройки богатого форматирования для заменённого текста.

```csharp
public FontSetting[] FontSettings { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyFontSettingsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите пример текста в ячейку A1
            worksheet.Cells["A1"].Value = "Sample text for replacement";
            
            // Создать параметры замены с настройками шрифта
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            
            // Создать настройку шрифта для заменяемого текста
            FontSetting fontSetting = new FontSetting(0, 8, workbook.Worksheets);
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Color = Color.Blue;
            
            // Применить настройки шрифта к параметрам замены
            options.FontSettings = new FontSetting[] { fontSetting };
            
            // Выполнить замену
            workbook.Replace("text", "REPLACED", options);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


