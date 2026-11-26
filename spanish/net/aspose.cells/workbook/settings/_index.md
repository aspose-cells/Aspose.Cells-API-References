---
title: "Workbook.Settings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Workbook. Representa la configuración del libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbook/settings/
---
## Workbook.Settings property

Representa la configuración del libro de trabajo.

```csharp
public WorkbookSettings Settings { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertySettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder y modificar la configuración
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 30;
            workbook.Settings.FormulaSettings.MaxChange = 0.1;

            // Verificar la configuración
            Console.WriteLine("Iterative Calculation Enabled: " + 
                workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + 
                workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + 
                workbook.Settings.FormulaSettings.MaxChange);

            // Guarda el libro de trabajo
            workbook.Save("WorkbookSettingsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


