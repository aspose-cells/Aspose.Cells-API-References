---
title: "PivotGlobalizationSettings.GetTextOfTotal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает текст метки Total в сводной таблице. Вам необходимо переопределить этот метод, когда сводная таблица содержит два или более PivotFields в области данных"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/
---
## PivotGlobalizationSettings.GetTextOfTotal method

Получает текст метки "Total" в сводной таблице. Вам необходимо переопределить этот метод, когда сводная таблица содержит два или более полей PivotFields в области данных.

```csharp
public virtual string GetTextOfTotal()
```

### Возвращаемое значение

Текст метки "Total"

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Создать и использовать настройки глобализации
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Продемонстрировать метод GetTextOfTotal
            Console.WriteLine("Total label text: " + globalizationSettings.GetTextOfTotal());

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


