---
title: "CalculationOptions.RefreshDynamicArrayFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationOptions. Indica si las fórmulas de matrices dinámicas deben refrescarse antes de calcular fórmulas"
type: docs
url: /es/net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

Indica si las fórmulas de matrices dinámicas deben actualizarse antes de calcular fórmulas.

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### Observaciones

Si esta propiedad se ha especificado explícitamente, entonces el valor especificado se usará para determinar si refrescar las fórmulas de matrices dinámicas. De lo contrario ([`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) es falso), el valor predeterminado depende del tipo de fórmulas que necesiten calcularse: para calcular fórmulas del libro de trabajo, como [`CalculateFormula`](../../workbook/calculateformula/), esta propiedad se considerará verdadera. En otros casos, como [`Calculate`](../../cell/calculate/) o [`CalculateFormula`](../../worksheet/calculateformula/), esta propiedad se considerará falsa.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una fórmula de matriz dinámica para demostrar la funcionalidad
            worksheet.Cells["A1"].Value = 1;
            worksheet.Cells["A2"].Value = 2;
            worksheet.Cells["A3"].Value = 3;
            worksheet.Cells["B1"].Formula = "=A1:A3"; // Dynamic array formula

            // Crear una instancia de CalculationOptions
            CalculationOptions options = new CalculationOptions();

            try
            {
                // Mostrar el valor predeterminado de RefreshDynamicArrayFormula
                Console.WriteLine("Default RefreshDynamicArrayFormula value: " + options.RefreshDynamicArrayFormula);

                // Establecer la propiedad a true para refrescar las fórmulas de matrices dinámicas
                options.RefreshDynamicArrayFormula = true;
                Console.WriteLine("After setting to true: " + options.RefreshDynamicArrayFormula);

                // Calcular fórmulas con las opciones especificadas
                workbook.CalculateFormula(options);

                // Mostrar el resultado calculado
                Console.WriteLine("Dynamic array formula result: " + worksheet.Cells["B1"].Value);

                // Guarda el libro de trabajo
                workbook.Save("RefreshDynamicArrayFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


