---
title: "GlobalizationSettings.GetSubTotalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает имя типа PivotFieldSubtotalType в сводной таблице"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getsubtotalname/
---
## GlobalizationSettings.GetSubTotalName method

Получает имя типа [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) в сводной таблице.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfSubTotal() method instead.")]
public virtual string GetSubTotalName(PivotFieldSubtotalType subTotalType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Тип [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Возвращаемое значение

Имя типа [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetSubTotalNameWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                var globalizationSettings = workbook.Settings.GlobalizationSettings;
                PivotFieldSubtotalType subtotalType = PivotFieldSubtotalType.Sum;
                string subTotalName = ((CustomGlobalizationSettings)globalizationSettings).GetSubTotalName(subtotalType);
                
                Console.WriteLine($"Subtotal name for {subtotalType}: {subTotalName}");
                workbook.Worksheets[0].Cells["A1"].PutValue(subTotalName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSubTotalName: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetSubTotalNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetSubTotalName(PivotFieldSubtotalType subTotalType)
            {
                return $"Custom {subTotalType}";
            }
        }
    }
}
```

### См. также

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


