---
title: "SettableChartGlobalizationSettings.GetAxisUnitName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Получает имя единицы оси"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/getaxisunitname/
---
## SettableChartGlobalizationSettings.GetAxisUnitName method

Получает название единицы оси.

```csharp
public override string GetAxisUnitName(DisplayUnitType type)
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте минимальные данные для контекста
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Создать экземпляр SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Вызовите GetAxisUnitName с разными значениями DisplayUnitType
                string hundredsUnit = settings.GetAxisUnitName(DisplayUnitType.Hundreds);
                string thousandsUnit = settings.GetAxisUnitName(DisplayUnitType.Thousands);
                string millionsUnit = settings.GetAxisUnitName(DisplayUnitType.Millions);
                string percentageUnit = settings.GetAxisUnitName(DisplayUnitType.Percentage);

                // Отобразите результаты
                Console.WriteLine($"Hundreds unit name: {hundredsUnit}");
                Console.WriteLine($"Thousands unit name: {thousandsUnit}");
                Console.WriteLine($"Millions unit name: {millionsUnit}");
                Console.WriteLine($"Percentage unit name: {percentageUnit}");

                // Сохраните книгу
                workbook.Save("GetAxisUnitNameDemo.xlsx");
                Console.WriteLine("GetAxisUnitName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetAxisUnitName: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


