---
title: "FormulaSettings.ForceFullCalculation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaSettings. Указывает, вычисляет ли он все формулы каждый раз, когда запускается расчёт"
type: docs
url: /ru/net/aspose.cells/formulasettings/forcefullcalculation/
---
## FormulaSettings.ForceFullCalculation property

Указывает, вычислять ли все формулы каждый раз при запуске вычисления.

```csharp
public bool ForceFullCalculation { get; set; }
```

### Примечания

Это свойство используется только для сохранения настроек в результирующий файл таблицы, чтобы другие приложения (например, MS Excel) могли соответствующим образом реагировать при загрузке и работе с этим файлом. С учётом производительности большинства пользовательских приложений мы не вычисляем автоматически ни одну формулу в книге, независимо от установленного значения этого свойства.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyForceFullCalculationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к настройкам формул
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Продемонстрировать свойство ForceFullCalculation
            formulaSettings.ForceFullCalculation = true;
            Console.WriteLine($"ForceFullCalculation is set to: {formulaSettings.ForceFullCalculation}");

            // Добавьте пример данных и формулу
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Вычислить формулы с настройкой ForceFullCalculation
            workbook.CalculateFormula();

            // Вывести результат.
            Console.WriteLine($"Calculation result: {worksheet.Cells["A3"].Value}");

            // Сохраните книгу
            workbook.Save("ForceFullCalculationDemo.xlsx");
        }
    }
}
```

### См. также

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


