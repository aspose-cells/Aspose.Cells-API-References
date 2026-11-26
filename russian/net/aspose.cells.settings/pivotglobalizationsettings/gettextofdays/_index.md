---
title: "PivotGlobalizationSettings.GetTextOfDays"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает локальный текст дней"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextofdays/
---
## PivotGlobalizationSettings.GetTextOfDays method

Получает локальный текст "Days".

```csharp
public virtual string GetTextOfDays()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfDaysDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B3"].PutValue(1500);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поле даты в область строк
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Создать настройки глобализации
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Продемонстрируйте метод GetTextOfDays
            Console.WriteLine("Localized text for days: " + globalizationSettings.GetTextOfDays());

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


