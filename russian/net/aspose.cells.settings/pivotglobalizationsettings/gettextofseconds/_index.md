---
title: "PivotGlobalizationSettings.GetTextOfSeconds"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает локальный текст для Seconds"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/
---
## PivotGlobalizationSettings.GetTextOfSeconds method

Получает локальный текст "Seconds"

```csharp
public virtual string GetTextOfSeconds()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfSecondsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(100);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B2", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поле даты в область строк
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Создать настройки глобализации
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Продемонстрировать метод GetTextOfSeconds
            Console.WriteLine("Localized text for seconds: " + globalizationSettings.GetTextOfSeconds());

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


