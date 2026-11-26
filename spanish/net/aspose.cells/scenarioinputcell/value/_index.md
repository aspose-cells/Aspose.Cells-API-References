---
title: "ScenarioInputCell.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScenarioInputCell. Obtiene y establece el valor de la celda de entrada"
type: docs
url: /es/net/aspose.cells/scenarioinputcell/value/
---
## ScenarioInputCell.Value property

Obtiene y establece el valor de la celda de entrada.

```csharp
public string Value { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un escenario
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Agregar celdas de entrada con valores
            scenario.InputCells.Add(0, 0, "100"); // Cell A1
            scenario.InputCells.Add(1, 1, "200"); // Cell B2

            // Acceder y modificar valores
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"Original value: {cell1.Value}");
            cell1.Value = "150"; // Modify the value
            Console.WriteLine($"Modified value: {cell1.Value}");

            // Guarda el libro de trabajo
            workbook.Save("ScenarioValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


