---
title: "Workbook.Settings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Представляет настройки workbook"
type: docs
url: /ru/net/aspose.cells/workbook/settings/
---
## Workbook.Settings property

Представляет настройки рабочей книги.

```csharp
public WorkbookSettings Settings { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertySettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Доступ к настройкам и их изменение
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 30;
            workbook.Settings.FormulaSettings.MaxChange = 0.1;

            // Проверить настройки
            Console.WriteLine("Iterative Calculation Enabled: " + 
                workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + 
                workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + 
                workbook.Settings.FormulaSettings.MaxChange);

            // Сохраните книгу
            workbook.Save("WorkbookSettingsDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


