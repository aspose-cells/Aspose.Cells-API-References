---
title: "Clase Scenario"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Scenario. Representa un escenario individual"
type: docs
url: /es/net/aspose.cells/scenario/
---
## Scenario class

Representa un escenario individual.

```csharp
public class Scenario
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Comment](../../aspose.cells/scenario/comment/) { get; set; } | Obtiene y establece el comentario del escenario. |
| [InputCells](../../aspose.cells/scenario/inputcells/) { get; } | Obtiene las celdas de entrada del escenario. |
| [IsHidden](../../aspose.cells/scenario/ishidden/) { get; set; } | Indica si el escenario está oculto. |
| [IsLocked](../../aspose.cells/scenario/islocked/) { get; set; } | Indica si el escenario está bloqueado para edición cuando la hoja está protegida. |
| [Name](../../aspose.cells/scenario/name/) { get; set; } | Obtiene y establece el nombre del escenario. |
| [User](../../aspose.cells/scenario/user/) { get; } | Obtiene el nombre del usuario que cambió el escenario por última vez. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioDemo
    {
        public static void ScenarioExample()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la colección de escenarios de la hoja de cálculo
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Agrega un nuevo escenario a la colección
            int scenarioIndex = scenarios.Add("MyScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // Estableciendo propiedades del escenario
            scenario.Comment = "This is a test scenario.";
            scenario.Name = "TestScenario";
            scenario.IsHidden = false;
            scenario.IsLocked = true;

            // Accediendo a propiedades de solo lectura
            string user = scenario.User;
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Guarda el libro de trabajo
            workbook.Save("ScenarioExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


