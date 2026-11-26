---
title: "SettableGlobalizationSettings.GetTotalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает общее имя конкретной функции"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/gettotalname/
---
## SettableGlobalizationSettings.GetTotalName method

Получает полное имя конкретной функции.

```csharp
public override string GetTotalName(ConsolidationFunction functionType)
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
    using System;

    public class SettableGlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Вызвать GetTotalName с ConsolidationFunction.Sum
                string totalName = globalizationSettings.GetTotalName(ConsolidationFunction.Sum);
                
                // Отобразить результат
                Console.WriteLine($"Total name for Sum function: {totalName}");

                // Добавить данные для демонстрации эффекта (хотя GetTotalName не изменяет таблицу)
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["B1"].PutValue("Total");
                worksheet.Cells["B4"].Formula = "=SUM(A2:A4)";
                
                // Вычислить формулы
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTotalName method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("SettableGlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


