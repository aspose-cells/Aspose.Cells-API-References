---
title: "FormulaSettings.CalculationId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaSettings. Указывает версию движка расчётов, используемого для вычисления значений в книге."
type: docs
url: /ru/net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

Указывает версию движка вычислений, используемого для расчёта значений в книге.

```csharp
public string CalculationId { get; set; }
```

### Примечания

Это свойство используется только для сохранения настроек в результирующий файл таблицы, чтобы другие приложения (например, MS Excel) могли соответствующим образом реагировать при загрузке и работе с этим файлом. В случае MS Excel, если значение этого свойства меньше идентификатора движка пересчёта, связанного с приложением, открывающим результирующий файл, приложение пересчитает результаты всех формул в этой книге сразу после загрузки файла. С учётом производительности большинства пользовательских приложений мы не вычисляем автоматически ни одну формулу в книге, независимо от установленного значения этого свойства.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationIdDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Установить формулу, поведение которой зависит от CalculationId
            Cell cell = sheet.Cells["A1"];
            cell.Formula = "=AND(\"a\",true)";
            
            // Вычислить без CalculationId (поведение по умолчанию)
            wb.CalculateFormula();
            Console.WriteLine("Without CalculationId: " + cell.Value);
            
            // Установить CalculationId и пересчитать
            wb.Settings.FormulaSettings.CalculationId = "181029";
            wb.CalculateFormula();
            Console.WriteLine("With CalculationId 181029: " + cell.BoolValue);
        }
    }
}
```

### См. также

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


