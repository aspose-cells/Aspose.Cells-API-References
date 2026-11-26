---
title: "SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает стандартное английское название стиля шрифта (Regular, Bold, Italic) для верхнего/нижнего колонтитула в соответствии с заданным локальным названием стиля шрифта"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Получает стандартное английское название стиля шрифта (Regular, Bold, Italic) для верхнего/нижнего колонтитула в соответствии с заданным названием стиля шрифта локали.

```csharp
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
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

    public class SettableGlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Установите сопоставление стандартного названия стиля шрифта для верхнего/нижнего колонтитула
            settings.SetStandardHeaderFooterFontStyleName("MyLocalFontStyle", "Arial");

            // Применить настройки к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Вызовите метод GetStandardHeaderFooterFontStyleName с локальным названием стиля шрифта
                string standardFontStyle = settings.GetStandardHeaderFooterFontStyleName("MyLocalFontStyle");
                
                // Отобразить результат
                Console.WriteLine($"Standard font style name for 'MyLocalFontStyle': {standardFontStyle}");

                // Создайте верхний колонтитул с локальным названием стиля шрифта
                worksheet.PageSetup.SetHeader(1, "&\"MyLocalFontStyle\"&12Test Header");

                // Покажите эффект в электронной таблице
                Console.WriteLine("Header set with local font style name 'MyLocalFontStyle'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


