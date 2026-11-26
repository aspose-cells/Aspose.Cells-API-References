---
title: "SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName method

Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции.

```csharp
public void SetStandardHeaderFooterFontStyleName(string localfontStyleName, string standardName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| localfontStyleName | String | Локальное название стиля шрифта для верхнего/нижнего колонтитула. |
| standardName | String | Стандартное имя функции (локаль en-US). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardHeaderFooterFontStyleNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте параметры настройки страницы для рабочего листа
            PageSetup pageSetup = worksheet.PageSetup;

            // Установите заголовок с некоторым текстом
            pageSetup.SetHeader(0, "&\"Arial\"&12This is a header");

            // Создайте экземпляр настроек глобализации
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Вызовите метод SetStandardHeaderFooterFontStyleName
                globalizationSettings.SetStandardHeaderFooterFontStyleName("Arial", "Times New Roman");

                // Примените настройки глобализации к рабочей книге
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                Console.WriteLine("SetStandardHeaderFooterFontStyleName method executed successfully with parameters (\"Arial\", \"Times New Roman\")");

                // Эффект будет виден при рендеринге или печати документа
                // Шрифт "Arial" в заголовках/колонтитулах будет восприниматься как "Times New Roman"
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("MethodSetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


