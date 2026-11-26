---
title: "SettablePivotGlobalizationSettings.SetTextOfSubTotal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettablePivotGlobalizationSettings. Устанавливает текст типа PivotFieldSubtotalType в сводной таблице"
type: docs
url: /ru/net/aspose.cells/settablepivotglobalizationsettings/settextofsubtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfSubTotal method

Устанавливает текст типа [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) в сводной таблице.

```csharp
public void SetTextOfSubTotal(PivotFieldSubtotalType subTotalType, string text)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Тип [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |
| текст | String | Текст указанного типа |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfSubTotalWithPivotFieldSubtoStringDemo
    {
        public static void Run()
        {
            // Создайте новую рабочую книгу (только для демонстрационных целей)
            Workbook workbook = new Workbook();

            // Экземпляр SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Установите пользовательский текст для подытога Sum
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum Total");

                // Проверьте изменение
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal text after change: {sumText}");

                // Установите пользовательский текст для подытога Average
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Average Total");

                // Проверьте изменение
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal text after change: {avgText}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfSubTotal: {ex.Message}");
            }

            // Сохраните рабочую книгу (в этой демонстрации нет изменений сводной таблицы)
            workbook.Save("SetTextOfSubTotalDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


