---
title: "CustomRenderSettings.CustomRenderSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор CustomRenderSettings. Ctor"
type: docs
url: /ru/net/aspose.cells.rendering/customrendersettings/customrendersettings/
---
## CustomRenderSettings constructor

Конструктор.

```csharp
public CustomRenderSettings()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для контекста
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";

            try
            {
                // Создайте экземпляр CustomRenderSettings с помощью конструктора
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Отобразите подтверждение успешного вызова конструктора
                Console.WriteLine("CustomRenderSettings instance created successfully using #ctor");

                // Продемонстрируйте, что экземпляр работает, вызвав метод
                float borderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                Console.WriteLine($"Default thin border width: {borderWidth}");

                // Сохраните книгу
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomRenderSettings: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


