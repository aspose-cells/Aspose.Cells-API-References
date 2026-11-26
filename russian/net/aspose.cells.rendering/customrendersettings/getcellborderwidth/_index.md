---
title: "CustomRenderSettings.GetCellBorderWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomRenderSettings. Указывает ширину границы ячейки в зависимости от типа границы"
type: docs
url: /ru/net/aspose.cells.rendering/customrendersettings/getcellborderwidth/
---
## CustomRenderSettings.GetCellBorderWidth method

Указывает ширину границы ячейки в зависимости от типа границы.

```csharp
public virtual float GetCellBorderWidth(CellBorderType borderType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| borderType | CellBorderType | тип границы ячейки |

### Возвращаемое значение

ширина границы ячейки

### Примечания

Любое отрицательное значение будет игнорироваться.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodGetCellBorderWidthWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для контекста
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Создайте экземпляр CustomRenderSettings
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Вызовите GetCellBorderWidth с разными типами границ
                float thinBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Отобразите результаты
                Console.WriteLine($"Thin border width: {thinBorderWidth}");
                Console.WriteLine($"Thick border width: {thickBorderWidth}");
                Console.WriteLine($"Dashed border width: {dashedBorderWidth}");

                // Сохраните книгу
                workbook.Save("GetCellBorderWidthDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [CellBorderType](../../../aspose.cells/cellbordertype/)
* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


