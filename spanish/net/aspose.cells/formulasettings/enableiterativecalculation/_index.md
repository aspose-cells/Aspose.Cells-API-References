---
title: "FormulaSettings.EnableIterativeCalculation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. Indica si se debe habilitar el cálculo iterativo para resolver referencias circulares"
type: docs
url: /es/net/aspose.cells/formulasettings/enableiterativecalculation/
---
## FormulaSettings.EnableIterativeCalculation property

Indica si se debe habilitar el cálculo iterativo para resolver referencias circulares.

```csharp
public bool EnableIterativeCalculation { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableIterativeCalculationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configurar una referencia circular para la demostración
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Habilitar el cálculo iterativo con el número máximo de iteraciones
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;
            
            // Calcular fórmulas
            workbook.CalculateFormula();
            
            // Mostrar resultados
            Console.WriteLine("A1 value after calculation: " + worksheet.Cells["A1"].DoubleValue);
            Console.WriteLine("B1 value after calculation: " + worksheet.Cells["B1"].DoubleValue);
        }
    }
}
```

### Ver también

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


