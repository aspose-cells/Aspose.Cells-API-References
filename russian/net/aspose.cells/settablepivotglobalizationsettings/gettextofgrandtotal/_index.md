---
title: "SettablePivotGlobalizationSettings.GetTextOfGrandTotal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettablePivotGlobalizationSettings. Получает текст метки Grand Total в сводной таблице"
type: docs
url: /ru/net/aspose.cells/settablepivotglobalizationsettings/gettextofgrandtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfGrandTotal method

Получает текст метки "Grand Total" в сводной таблице.

```csharp
public override string GetTextOfGrandTotal()
```

### Возвращаемое значение

Текст метки "Grand Total"

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfGrandTotalDemo
    {
        public static void Run()
        {
            // Создайте новую рабочую книгу (только для контекста)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample");

            // Экземпляр SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Измените текст по умолчанию для "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Получите текущий текст "Grand Total"
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Сохраните книгу (сводная таблица не создаётся, но файл сохраняется для подтверждения выполнения)
                workbook.Save("GetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


