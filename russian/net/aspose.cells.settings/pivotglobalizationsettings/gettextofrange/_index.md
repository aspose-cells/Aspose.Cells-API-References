---
title: "PivotGlobalizationSettings.GetTextOfRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает локальный текст Range"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextofrange/
---
## PivotGlobalizationSettings.GetTextOfRange method

Получает локальный текст "Range"

```csharp
public virtual string GetTextOfRange()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Создайте настройки глобализации и продемонстрируйте GetTextOfRange
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            Console.WriteLine("Text of Range: " + globalizationSettings.GetTextOfRange());

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


