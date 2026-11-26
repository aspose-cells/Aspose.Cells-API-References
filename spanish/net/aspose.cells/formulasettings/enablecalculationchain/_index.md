---
title: "FormulaSettings.EnableCalculationChain"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. Indica si se debe habilitar la cadena de cálculo para las fórmulas. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

Indica si se debe habilitar la cadena de cálculo para fórmulas. El valor predeterminado es false.

```csharp
public bool EnableCalculationChain { get; set; }
```

### Observaciones

Cuando hay muchas fórmulas en el libro de trabajo y el usuario necesita calcularlas repetidamente modificando solo una pequeña parte de ellas, puede ser útil para el rendimiento habilitar la cadena de cálculo. Por otro lado, si la cadena está habilitada, mantener el modelo de cadena requiere memoria adicional y también necesita un poco más de tiempo de CPU para algunas otras operaciones, como cambiar el valor de una celda o sus fórmulas. Después de cambiar esta propiedad de false a true, la cadena de cálculo se analizará y construirá en el momento del primer cálculo del libro de trabajo, por lo que el tiempo requerido para el primer cálculo puede ser mayor que el cálculo normal sin cadena.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableCalculationChainDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar fórmulas de ejemplo
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
            
            // Desactivar cadena de cálculo
            workbook.Settings.FormulaSettings.EnableCalculationChain = false;
            
            // Calcular fórmulas
            workbook.CalculateFormula();
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with calculation chain disabled.");
        }
    }
}
```

### Ver también

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


