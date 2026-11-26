---
title: "GlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает стандартное английское название стиля шрифта Regular Bold Italic для Header/Footer в соответствии с заданным локальным названием стиля шрифта"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/
---
## GlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Получает стандартное английское название стиля шрифта (Regular, Bold, Italic) для верхнего/нижнего колонтитула в соответствии с заданным названием стиля шрифта локали.

```csharp
public virtual string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| localfontStyleName | String | Локальное название стиля шрифта для верхнего/нижнего колонтитула. |

### Возвращаемое значение

Стандартное английское название стиля шрифта (Regular, Bold, Italic)

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр пользовательских настроек глобализации
            var globalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Продемонстрировать вызов метода с параметром типа (String)
                string localStyle = "CustomBold";
                string standardStyle = globalizationSettings.GetStandardHeaderFooterFontStyleName(localStyle);
                Console.WriteLine($"Converted font style: {localStyle} -> {standardStyle}");

                // Применить настройки глобализации к рабочей книге
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Установить заголовок с пользовательским стилем шрифта, который будет преобразован
                // Использовать метод SetHeader с параметром section (0 = слева, 1 = центр, 2 = справа)
                worksheet.PageSetup.SetHeader(1, "&\"Arial\"&\"CustomBold\"&12Header Text");

                // Сохранить рабочую книгу, чтобы продемонстрировать эффект
                workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
        }
    }

    // Реализация пользовательских настроек глобализации
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
        {
            // Преобразовать пользовательские названия стилей шрифта в стандартные названия
            return localfontStyleName switch
            {
                "CustomBold" => "Bold",
                "CustomItalic" => "Italic",
                _ => base.GetStandardHeaderFooterFontStyleName(localfontStyleName)
            };
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


