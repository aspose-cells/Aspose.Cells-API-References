---
title: "FormulaSettings.PrecisionAsDisplayed"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. Indica si la precisión del resultado calculado se establece según se muestra al calcular fórmulas"
type: docs
url: /es/net/aspose.cells/formulasettings/precisionasdisplayed/
---
## FormulaSettings.PrecisionAsDisplayed property

Indica si la precisión del resultado calculado se establece como se muestra al calcular fórmulas.

```csharp
public bool PrecisionAsDisplayed { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPrecisionAsDisplayedDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer PrecisionAsDisplayed en true
            workbook.Settings.FormulaSettings.PrecisionAsDisplayed = true;
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Establecer el formato de visualización de la celda A1 para mostrar 2 decimales
            cells["A1"].PutValue(1.23456);
            Style style = cells["A1"].GetStyle();
            style.Number = 2; // Format: 0.00
            cells["A1"].SetStyle(style);
            
            // Establecer una fórmula en B1 que haga referencia a A1
            cells["B1"].Formula = "=A1";
            
            // Calcular fórmulas con PrecisionAsDisplayed habilitado
            workbook.CalculateFormula();
            
            // Mostrar resultados
            Console.WriteLine("A1 Display Value: " + cells["A1"].StringValue); // Shows 1.23
            Console.WriteLine("B1 Calculated Value: " + cells["B1"].Value);   // Should be 1.23 due to PrecisionAsDisplayed
        }
    }
}
```

### Ver también

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


