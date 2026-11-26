---
title: "Clase FormulaSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FormulaSettings. Configuraciones de fórmulas y cálculo"
type: docs
url: /es/net/aspose.cells/formulasettings/
---
## FormulaSettings class

Configuración de fórmulas y cálculo.

```csharp
public class FormulaSettings
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CalculateOnOpen](../../aspose.cells/formulasettings/calculateonopen/) { get; set; } | Indica si la aplicación debe realizar un cálculo completo cuando se abre el libro de trabajo. |
| [CalculateOnSave](../../aspose.cells/formulasettings/calculateonsave/) { get; set; } | Indica si se debe recalcular el libro de trabajo antes de guardar el documento, cuando está en modo de cálculo manual. |
| [CalculationId](../../aspose.cells/formulasettings/calculationid/) { get; set; } | Especifica la versión del motor de cálculo utilizado para calcular los valores en el libro de trabajo. |
| [CalculationMode](../../aspose.cells/formulasettings/calculationmode/) { get; set; } | Obtiene o establece el modo de cálculo del libro de trabajo en MS Excel. |
| [EnableCalculationChain](../../aspose.cells/formulasettings/enablecalculationchain/) { get; set; } | Indica si se debe habilitar la cadena de cálculo para fórmulas. El valor predeterminado es false. |
| [EnableIterativeCalculation](../../aspose.cells/formulasettings/enableiterativecalculation/) { get; set; } | Indica si se debe habilitar el cálculo iterativo para resolver referencias circulares. |
| [ForceFullCalculation](../../aspose.cells/formulasettings/forcefullcalculation/) { get; set; } | Indica si calcula todas las fórmulas cada vez que se desencadena un cálculo. |
| [MaxChange](../../aspose.cells/formulasettings/maxchange/) { get; set; } | El cambio máximo para resolver una referencia circular. |
| [MaxIteration](../../aspose.cells/formulasettings/maxiteration/) { get; set; } | El número máximo de iteraciones para resolver una referencia circular. |
| [PrecisionAsDisplayed](../../aspose.cells/formulasettings/precisionasdisplayed/) { get; set; } | Indica si la precisión del resultado calculado se establece como se muestra al calcular fórmulas. |
| [PreservePaddingSpaces](../../aspose.cells/formulasettings/preservepaddingspaces/) { get; set; } | Indica si se deben conservar los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es false. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaSettingsDemo
    {
        public static void FormulaSettingsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la configuración de fórmulas del libro de trabajo
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Estableciendo propiedades
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationMode = CalcModeType.Automatic;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Guarda el libro de trabajo
            workbook.Save("FormulaSettingsExample.xlsx");
            workbook.Save("FormulaSettingsExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


