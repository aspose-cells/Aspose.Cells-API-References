---
title: "FormulaSettings.CalculationId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. Especifica la versión del motor de cálculo utilizado para calcular los valores en el libro de trabajo"
type: docs
url: /es/net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

Especifica la versión del motor de cálculo utilizado para calcular los valores en el libro de trabajo.

```csharp
public string CalculationId { get; set; }
```

### Observaciones

Esta propiedad solo sirve para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como MS Excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. En el caso de MS Excel, si el valor de esta propiedad es menor que el identificador del motor de recálculo asociado con la aplicación que abre el archivo resultante, la aplicación recalculará los resultados de todas las fórmulas en este libro de trabajo inmediatamente después de cargar el archivo. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos automáticamente ninguna fórmula en el libro de trabajo, sin importar el valor que se haya establecido para esta propiedad.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationIdDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Establecer fórmula que se comporte de manera diferente según CalculationId
            Cell cell = sheet.Cells["A1"];
            cell.Formula = "=AND(\"a\",true)";
            
            // Calcular sin CalculationId (comportamiento predeterminado)
            wb.CalculateFormula();
            Console.WriteLine("Without CalculationId: " + cell.Value);
            
            // Establecer CalculationId y recalcular
            wb.Settings.FormulaSettings.CalculationId = "181029";
            wb.CalculateFormula();
            Console.WriteLine("With CalculationId 181029: " + cell.BoolValue);
        }
    }
}
```

### Ver también

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


