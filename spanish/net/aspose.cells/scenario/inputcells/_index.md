---
title: "Scenario.InputCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Scenario. Obtiene las celdas de entrada del escenario"
type: docs
url: /es/net/aspose.cells/scenario/inputcells/
---
## Scenario.InputCells property

Obtiene las celdas de entrada del escenario.

```csharp
public ScenarioInputCellCollection InputCells { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyInputCellsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un escenario a la hoja de cálculo
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Agregar celdas de entrada al escenario usando la propiedad InputCells
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Cell A1
            inputCells.Add(1, 1, "200"); // Cell B2

            // Modificar el valor de la primera celda de entrada
            inputCells[0].Value = "150";

            // Guarda el libro de trabajo
            workbook.Save("ScenarioInputCellsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ScenarioInputCellCollection](../../scenarioinputcellcollection/)
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


