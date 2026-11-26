---
title: "ReplaceOptions.StyleFlags"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ReplaceOptions свойство. Получает и задает флаги применения настроек шрифта"
type: docs
url: /ru/net/aspose.cells/replaceoptions/styleflags/
---
## ReplaceOptions.StyleFlags property

Получает и задаёт флаги применения настроек шрифта.

```csharp
public StyleFlag[] StyleFlags { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyStyleFlagsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить образец текста в ячейку
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("test text");

            // Создать параметры замены
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            options.CaseSensitive = false;

            // Создать настройку шрифта и флаг стиля
            string replacementText = "new text";
            FontSetting setting = new FontSetting(0, replacementText.Length, workbook.Worksheets);
            StyleFlag styleFlag = new StyleFlag();
            
            // Настроить шрифт и стиль
            setting.Font.Color = Color.Red;
            setting.Font.Underline = FontUnderlineType.Single;
            styleFlag.FontColor = true;
            styleFlag.FontUnderline = true;

            // Применить настройки к параметрам
            options.FontSettings = new FontSetting[] { setting };
            options.StyleFlags = new StyleFlag[] { styleFlag };

            // Выполнить замену
            workbook.Replace("test", replacementText, options);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


