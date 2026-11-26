---
title: "FormulaSettings.MaxChange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaSettings. Максимальное изменение для разрешения циклической ссылки"
type: docs
url: /ru/net/aspose.cells/formulasettings/maxchange/
---
## FormulaSettings.MaxChange property

Максимальное изменение для разрешения циклической ссылки.

```csharp
public double MaxChange { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyMaxChangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Настроить параметры итеративного расчёта
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001; // Set maximum change threshold
            
            // Создать циклическую ссылку для демонстрации
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Вычислить формулы с указанной настройкой MaxChange
            workbook.CalculateFormula();
            
            // Вывести результаты
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("MaxChange used: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### См. также

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


