---
title: "FormulaSettings.MaxChange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. El cambio máximo para resolver una referencia circular"
type: docs
url: /es/net/aspose.cells/formulasettings/maxchange/
---
## FormulaSettings.MaxChange property

El cambio máximo para resolver una referencia circular.

```csharp
public double MaxChange { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyMaxChangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configurar los ajustes de cálculo iterativo
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001; // Set maximum change threshold
            
            // Crear una referencia circular para demostración
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Calcular fórmulas con el ajuste MaxChange especificado
            workbook.CalculateFormula();
            
            // Mostrar resultados
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("MaxChange used: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### Ver también

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


