---
title: "WorkbookSettings.FormulaSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает настройки, связанные с формулами"
type: docs
url: /ru/net/aspose.cells/workbooksettings/formulasettings/
---
## WorkbookSettings.FormulaSettings property

Получает настройки функций, связанных с формулами.

```csharp
public FormulaSettings FormulaSettings { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFormulaSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получите доступ и измените FormulaSettings
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;

            // Отобразите настройки
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
            Console.WriteLine("Iterative Calculation Enabled: " + workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### См. также

* class [FormulaSettings](../../formulasettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


