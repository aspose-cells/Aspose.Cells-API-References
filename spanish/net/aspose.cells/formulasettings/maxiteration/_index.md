---
title: "FormulaSettings.MaxIteration"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. El número máximo de iteraciones para resolver una referencia circular"
type: docs
url: /es/net/aspose.cells/formulasettings/maxiteration/
---
## FormulaSettings.MaxIteration property

El número máximo de iteraciones para resolver una referencia circular.

```csharp
public int MaxIteration { get; set; }
```

### Ejemplos

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

### Ver también

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


