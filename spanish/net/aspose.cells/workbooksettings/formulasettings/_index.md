---
title: "WorkbookSettings.FormulaSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene la configuración de las funciones relacionadas con fórmulas"
type: docs
url: /es/net/aspose.cells/workbooksettings/formulasettings/
---
## WorkbookSettings.FormulaSettings property

Obtiene la configuración de las funciones relacionadas con fórmulas.

```csharp
public FormulaSettings FormulaSettings { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFormulaSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceda y modifique FormulaSettings
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;

            // Muestre la configuración
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
            Console.WriteLine("Iterative Calculation Enabled: " + workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### Ver también

* class [FormulaSettings](../../formulasettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


