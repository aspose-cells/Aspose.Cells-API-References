---
title: "FormulaSettings.MaxIteration"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaSettings. Максимальное количество итераций для разрешения циклической ссылки"
type: docs
url: /ru/net/aspose.cells/formulasettings/maxiteration/
---
## FormulaSettings.MaxIteration property

Максимальное количество итераций для разрешения циклической ссылки.

```csharp
public int MaxIteration { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyMaxIterationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 10;
            
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].Formula = "=A2+1";
            cells["A2"].Formula = "=A1+1";
            
            workbook.CalculateFormula();
            
            Console.WriteLine("A1 value: " + cells["A1"].Value);
            Console.WriteLine("A2 value: " + cells["A2"].Value);
        }
    }
}
```

### См. также

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


