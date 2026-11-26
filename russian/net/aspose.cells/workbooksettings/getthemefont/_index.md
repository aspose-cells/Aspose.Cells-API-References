---
title: "WorkbookSettings.GetThemeFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorkbookSettings. Возвращает имя шрифта темы по умолчанию"
type: docs
url: /ru/net/aspose.cells/workbooksettings/getthemefont/
---
## WorkbookSettings.GetThemeFont method

Получает имя шрифта темы по умолчанию.

```csharp
public string GetThemeFont(FontSchemeType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | FontSchemeType | Тип схемы шрифта. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodGetThemeFontWithFontSchemeTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить шрифт темы по умолчанию для типа схемы minor
            string minorFont = workbook.Settings.GetThemeFont(FontSchemeType.Minor);
            Console.WriteLine("Minor theme font: " + minorFont);
            
            // Получить шрифт темы по умолчанию для типа схемы major
            string majorFont = workbook.Settings.GetThemeFont(FontSchemeType.Major);
            Console.WriteLine("Major theme font: " + majorFont);
            
            // Сохраните книгу
            workbook.Save("ThemeFontExample.xlsx");
        }
    }
}
```

### См. также

* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


