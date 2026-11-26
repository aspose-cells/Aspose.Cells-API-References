---
title: "SettablePivotGlobalizationSettings.GetTextOfSubTotal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettablePivotGlobalizationSettings. Получает текст типа PivotFieldSubtotalType в сводной таблице"
type: docs
url: /ru/net/aspose.cells/settablepivotglobalizationsettings/gettextofsubtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfSubTotal method

Получает текст типа [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) в сводной таблице.

```csharp
public override string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Тип [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Возвращаемое значение

Текст указанного типа

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfSubTotalWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Вызовите GetTextOfSubTotal с разными значениями PivotFieldSubtotalType
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                string countText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Count);

                // Отобразите результаты
                Console.WriteLine($"Sum subtotal text: {sumText}");
                Console.WriteLine($"Average subtotal text: {avgText}");
                Console.WriteLine($"Count subtotal text: {countText}");

                // Установите пользовательский текст для промежуточных итогов
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum");
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Avg");

                // Проверить изменения
                Console.WriteLine($"Modified Sum text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum)}");
                Console.WriteLine($"Modified Avg text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfSubTotal method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("SettablePivotGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


