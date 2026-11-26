---
title: "SettablePivotGlobalizationSettings.SetTextOfGrandTotal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettablePivotGlobalizationSettings. Устанавливает текст метки Grand Total в сводной таблице"
type: docs
url: /ru/net/aspose.cells/settablepivotglobalizationsettings/settextofgrandtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfGrandTotal method

Устанавливает текст метки "Grand Total" в сводной таблице.

```csharp
public void SetTextOfGrandTotal(string text)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | String | пользовательский текст |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalWithStringDemo
    {
        public static void Run()
        {
            // Создайте новую книгу (только контекст)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Экземпляр SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Установите пользовательский текст для метки "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Получите обновлённый текст метки, чтобы проверить изменение
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Сохраните книгу, просто чтобы продемонстрировать, что код выполняется без ошибок
                workbook.Save("SetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


