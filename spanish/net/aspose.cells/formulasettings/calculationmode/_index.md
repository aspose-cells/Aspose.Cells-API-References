---
title: "FormulaSettings.CalculationMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. Obtiene o establece el modo de cálculo del libro de trabajo en MS Excel"
type: docs
url: /es/net/aspose.cells/formulasettings/calculationmode/
---
## FormulaSettings.CalculationMode property

Obtiene o establece el modo de cálculo del libro de trabajo en MS Excel.

```csharp
public CalcModeType CalculationMode { get; set; }
```

### Observaciones

Esta propiedad solo sirve para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como MS Excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué modo se haya establecido para esta propiedad. Si el usuario necesita calcular fórmulas, por favor siempre invoque los métodos en diferentes objetos según el requerimiento: [`CalculateFormula`](../../workbook/calculateformula/), [`CalculateFormula`](../../worksheet/calculateformula/), [`Calculate`](../../cell/calculate/), ...etc.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationModeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer el modo de cálculo a AutomaticExceptTable
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.AutomaticExceptTable;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Cambiar el modo de cálculo a Manual
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Restablecer al modo Automatic predeterminado
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Automatic;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
        }
    }
}
```

### Ver también

* enum [CalcModeType](../../calcmodetype/)
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


