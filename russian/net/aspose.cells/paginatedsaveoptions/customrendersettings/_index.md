---
title: "PaginatedSaveOptions.CustomRenderSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Получает или задает пользовательские настройки во время рендеринга"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/customrendersettings/
---
## PaginatedSaveOptions.CustomRenderSettings property

Получает или задает пользовательские настройки во время рендеринга.

```csharp
public CustomRenderSettings CustomRenderSettings { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "This demonstrates CustomRenderSettings property";

            try
            {
                // Создайте PdfSaveOptions, который наследуется от PaginatedSaveOptions
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Получите текущее значение CustomRenderSettings
                CustomRenderSettings currentSettings = saveOptions.CustomRenderSettings;
                Console.WriteLine("Current CustomRenderSettings: " +
                    (currentSettings == null ? "null" : "CustomRenderSettings instance"));

                // Создайте и задайте новые CustomRenderSettings
                CustomRenderSettings newSettings = new CustomRenderSettings();
                saveOptions.CustomRenderSettings = newSettings;

                // Проверьте, что новые настройки были применены
                Console.WriteLine("New CustomRenderSettings set: " +
                    (saveOptions.CustomRenderSettings == newSettings ? "Success" : "Failed"));

                // Сохраните книгу с пользовательскими настройками рендеринга
                workbook.Save("CustomRenderSettingsDemo.pdf", saveOptions);
                Console.WriteLine("Workbook saved with CustomRenderSettings");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomRenderSettings](../../../aspose.cells.rendering/customrendersettings/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


