---
title: "CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationOptions. Indica si el usuario ha especificado explícitamente el comportamiento de refrescar fórmulas de matrices dinámicas antes de calcular fórmulas especificadas"
type: docs
url: /es/net/aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/
---
## CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property

Indica si el usuario ha especificado explícitamente el comportamiento de actualizar las fórmulas de matrices dinámicas antes de calcular fórmulas especificadas.

```csharp
public bool UserSpecifiedRefreshDynamicArrayFormula { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyUserSpecifiedRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crear una instancia de CalculationOptions
                CalculationOptions options = new CalculationOptions();

                // Mostrar el valor actual de la propiedad UserSpecifiedRefreshDynamicArrayFormula
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula value: " +
                    options.UserSpecifiedRefreshDynamicArrayFormula);

                // Mostrar cómo la propiedad afecta el comportamiento
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula has been demonstrated");

                // Guardar el resultado
                workbook.Save("UserSpecifiedRefreshDynamicArrayFormulaDemo.xlsx");
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


