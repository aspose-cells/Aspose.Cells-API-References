---
title: "GlobalizationSettings.GetProtectionNameOfPivotTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает имя защиты в сводной таблице"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getprotectionnameofpivottable/
---
## GlobalizationSettings.GetProtectionNameOfPivotTable method

Получает имя защиты в сводной таблице.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetProtectionNameOfPivotTable()
```

### Возвращаемое значение

Имя защиты сводной таблицы

### Примечания

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо этого, пожалуйста, используйте метод PivotGlobalizationSettings.GetTextOfProtectedName(string). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать стандартные параметры глобализации
            GlobalizationSettings standardSettings = new GlobalizationSettings();
            
            // Создайте пользовательские настройки глобализации
            GlobalizationSettings customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Получить имя защиты по умолчанию
                string defaultName = standardSettings.GetProtectionNameOfPivotTable();
                Console.WriteLine($"Default protection name: {defaultName}");

                // Получить имя пользовательской защиты
                string customName = customSettings.GetProtectionNameOfPivotTable();
                Console.WriteLine($"Custom protection name: {customName}");

                // Создать сводную таблицу для демонстрации применения параметров
                worksheet.Cells["A1"].Value = "Data";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;
                int pivotIndex = worksheet.PivotTables.Add("A1", "A1:A4", "PivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Защита обычно применяется здесь с использованием полученного имени
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetProtectionNameOfPivotTable: {ex.Message}");
            }
            
            workbook.Save("GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public new string GetProtectionNameOfPivotTable()
        {
            return "CustomPivotProtection";
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


