---
title: "ImageOrPrintOptions.CustomRenderSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает пользовательские настройки во время рендеринга"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/customrendersettings/
---
## ImageOrPrintOptions.CustomRenderSettings property

Получает или задает пользовательские настройки во время рендеринга.

```csharp
public CustomRenderSettings CustomRenderSettings { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class ImageOrPrintOptionsPropertyCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Создать новую рабочую книгу с некоторыми образцовыми данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo for CustomRenderSettings");
            sheet.Cells["B2"].PutValue(12345);
            sheet.Cells["C3"].PutValue(DateTime.Now);

            try
            {
                // Инициализировать ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Получить доступ к свойству CustomRenderSettings (read‑only) и отобразить его текущее состояние
                var customRenderSettings = options.CustomRenderSettings;
                Console.WriteLine("CustomRenderSettings instance: " +
                                  (customRenderSettings != null ? customRenderSettings.GetType().FullName : "null"));

                // При необходимости продемонстрировать, что параметры всё ещё работают при рендеринге
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                SheetRender renderer = new SheetRender(sheet, options);
                renderer.ToImage(0, "CustomRenderSettingsDemo.png");

                Console.WriteLine("Image rendered successfully.");
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

* class [CustomRenderSettings](../../customrendersettings/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


