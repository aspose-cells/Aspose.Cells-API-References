---
title: "PivotGlobalizationSettings.GetTextOfRowLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает текст метки Row Labels в сводной таблице"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/
---
## PivotGlobalizationSettings.GetTextOfRowLabels method

Получает текст метки "Row Labels" в сводной таблице.

```csharp
public virtual string GetTextOfRowLabels()
```

### Возвращаемое значение

Текст меток строк

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B3"].PutValue(200);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Создать и использовать настройки глобализации
            PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
            
            // Продемонстрировать GetTextOfRowLabels
            Console.WriteLine("Row Labels Text: " + settings.GetTextOfRowLabels());

            // Сохраните книгу
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


