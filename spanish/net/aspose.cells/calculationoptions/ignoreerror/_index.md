---
title: "CalculationOptions.IgnoreError"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationOptions. Indica si los errores encontrados al calcular fórmulas deben ser ignorados. El error puede ser una función no compatible, enlaces externos, etc. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

Indica si los errores encontrados al calcular fórmulas deben ser ignorados. El error puede ser una función no compatible, enlaces externos, etc. El valor predeterminado es true.

```csharp
public bool IgnoreError { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un rango con nombre que no exista para demostrar el manejo de errores
            worksheet.Cells["A1"].Formula = "=NONEXISTENTNAME()";
            
            // Calcular con IgnoreError = false (generará un error)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = false });
                Console.WriteLine("Calculation completed without ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (expected): " + ex.Message);
            }

            // Calcular con IgnoreError = true (suprimirá el error)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = true });
                Console.WriteLine("Calculation completed while ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (unexpected): " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


