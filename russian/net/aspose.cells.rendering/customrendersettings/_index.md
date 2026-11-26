---
title: "Класс CustomRenderSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.CustomRenderSettings. Представляет пользовательские настройки во время рендеринга"
type: docs
url: /ru/net/aspose.cells.rendering/customrendersettings/
---
## CustomRenderSettings class

Представляет пользовательские настройки во время рендеринга.

```csharp
public class CustomRenderSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CustomRenderSettings](customrendersettings/)() | Конструктор. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [GetCellBorderWidth](../../aspose.cells.rendering/customrendersettings/getcellborderwidth/)(CellBorderType) | Указывает ширину границы ячейки в зависимости от типа границы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "Border Width Test";

            try
            {
                // Создайте экземпляр CustomRenderSettings, используя конструктор по умолчанию
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Продемонстрируйте метод GetCellBorderWidth с различными типами границ
                float thinWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Отобразите результаты
                Console.WriteLine($"Thin border width: {thinWidth}");
                Console.WriteLine($"Thick border width: {thickWidth}");
                Console.WriteLine($"Dashed border width: {dashedWidth}");

                // Сохраните книгу
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("CustomRenderSettings demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CustomRenderSettings demonstration: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


