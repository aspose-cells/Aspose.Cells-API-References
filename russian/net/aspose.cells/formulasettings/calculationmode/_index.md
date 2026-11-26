---
title: "FormulaSettings.CalculationMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaSettings. Получает или задает режим расчёта книги в MS Excel"
type: docs
url: /ru/net/aspose.cells/formulasettings/calculationmode/
---
## FormulaSettings.CalculationMode property

Получает или задаёт режим вычисления книги в MS Excel.

```csharp
public CalcModeType CalculationMode { get; set; }
```

### Примечания

Это свойство предназначено только для сохранения настроек в результирующий файл таблицы, чтобы другие приложения (например, ms excel) могли соответствующим образом реагировать при загрузке и работе с результирующим файлом. По соображениям производительности большинства пользовательских приложений мы не вычисляем формулы в книге автоматически, независимо от того, какой режим установлен для этого свойства. Если пользователю необходимо вычислять формулы, пожалуйста, всегда вызывайте методы разных объектов в соответствии с требованием: [`CalculateFormula`](../../workbook/calculateformula/), [`CalculateFormula`](../../worksheet/calculateformula/), [`Calculate`](../../cell/calculate/), ...etc.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationModeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установить режим расчёта в AutomaticExceptTable
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.AutomaticExceptTable;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Изменить режим расчёта на Manual
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Сбросить к режиму Automatic по умолчанию
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Automatic;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
        }
    }
}
```

### См. также

* enum [CalcModeType](../../calcmodetype/)
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


