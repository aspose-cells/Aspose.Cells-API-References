---
title: "FormulaSettings.EnableCalculationChain"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaSettings. Указывает, следует ли включить цепочку расчётов для формул. По умолчанию false."
type: docs
url: /ru/net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

Указывает, включить ли цепочку вычислений для формул. По умолчанию — false.

```csharp
public bool EnableCalculationChain { get; set; }
```

### Примечания

Когда в книге много формул и пользователю требуется многократно их вычислять, изменяя лишь небольшую часть, включение цепочки расчётов может улучшить производительность. С другой стороны, если цепочка включена, поддержание её модели требует дополнительной памяти и немного больше процессорного времени для некоторых операций, таких как изменение значения ячейки или формул. После изменения этого свойства с false на true цепочка расчётов будет проанализирована и построена во время первого вычисления книги, поэтому время, необходимое для первого расчёта, может быть больше, чем при обычном расчёте без цепочки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableCalculationChainDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные формулы
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
            
            // Отключить цепочку расчётов
            workbook.Settings.FormulaSettings.EnableCalculationChain = false;
            
            // Вычислить формулы
            workbook.CalculateFormula();
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with calculation chain disabled.");
        }
    }
}
```

### См. также

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


