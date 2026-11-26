---
title: "GlobalizationSettings.PivotSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GlobalizationSettings. Получает или задает параметры глобализации для сводной таблицы"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/pivotsettings/
---
## GlobalizationSettings.PivotSettings property

Получает или задаёт настройки глобализации для сводной таблицы.

```csharp
public PivotGlobalizationSettings PivotSettings { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfTotal()
        {
            return "Custom Total";
        }

        public override string GetTextOfGrandTotal()
        {
            return "Custom Grand Total";
        }

        public override string GetTextOfDataFieldHeader()
        {
            return "DataCaption";
        }

        public override string GetTextOfProtectedName(string protectedName)
        {
            return protectedName + "2";
        }
    }

    public class GlobalizationSettingsPropertyPivotSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Orange");
            dataSheet.Cells["B3"].PutValue(2000);

            // Создать сводную таблицу
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int index = pivotSheet.PivotTables.Add("A1", "A1:B3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];
            
            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Установить пользовательские настройки глобализации для сводной таблицы
            CustomPivotGlobalizationSettings pivotSettings = new CustomPivotGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = new GlobalizationSettings();
            workbook.Settings.GlobalizationSettings.PivotSettings = pivotSettings;

            // Обновить сводную таблицу, чтобы применить настройки
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotGlobalizationSettings](../../../aspose.cells.settings/pivotglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


