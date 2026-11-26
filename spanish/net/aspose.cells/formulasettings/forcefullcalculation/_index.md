---
title: "FormulaSettings.ForceFullCalculation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. Indica si calcula todas las fórmulas cada vez que se desencadena un cálculo"
type: docs
url: /es/net/aspose.cells/formulasettings/forcefullcalculation/
---
## FormulaSettings.ForceFullCalculation property

Indica si calcula todas las fórmulas cada vez que se desencadena un cálculo.

```csharp
public bool ForceFullCalculation { get; set; }
```

### Observaciones

Esta propiedad solo sirve para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como MS Excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos automáticamente ninguna fórmula en el libro de trabajo, sin importar el valor que se haya establecido para esta propiedad.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyForceFullCalculationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración de fórmulas
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Demostrar la propiedad ForceFullCalculation
            formulaSettings.ForceFullCalculation = true;
            Console.WriteLine($"ForceFullCalculation is set to: {formulaSettings.ForceFullCalculation}");

            // Agregar datos de muestra y fórmula
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Calcular fórmulas con la configuración ForceFullCalculation
            workbook.CalculateFormula();

            // Mostrar el resultado
            Console.WriteLine($"Calculation result: {worksheet.Cells["A3"].Value}");

            // Guarda el libro de trabajo
            workbook.Save("ForceFullCalculationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


