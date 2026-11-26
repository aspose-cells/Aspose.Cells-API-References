---
title: "GlobalizationSettings.GetTotalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает полное имя функции."
type: docs
url: /ru/net/aspose.cells/globalizationsettings/gettotalname/
---
## GlobalizationSettings.GetTotalName method

Получает общее имя функции.

```csharp
public virtual string GetTotalName(ConsolidationFunction functionType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| functionType | ConsolidationFunction | Тип функции. |

### Возвращаемое значение

Общее имя функции.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;

            // Создайте пользовательские настройки глобализации
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Демонстрировать прямой вызов метода
                Console.WriteLine("Sum Total Name: " + 
                    customSettings.GetTotalName(ConsolidationFunction.Sum));
                
                // Создать сводную таблицу, чтобы вызвать использование GetTotalName
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                PivotField dataField = pivotTable.DataFields[dataFieldIndex];
                dataField.Function = ConsolidationFunction.Sum;

                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom total names");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTotalName(ConsolidationFunction functionType)
            {
                return functionType switch
                {
                    ConsolidationFunction.Sum => "[Sum Custom]",
                    ConsolidationFunction.Count => "[Count Custom]",
                    _ => base.GetTotalName(functionType)
                };
            }
        }
    }
}
```

### См. также

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


