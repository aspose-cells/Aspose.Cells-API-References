---
title: "ScenarioInputCell.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScenarioInputCell. Obtiene y establece la dirección de la celda de entrada"
type: docs
url: /es/net/aspose.cells/scenarioinputcell/name/
---
## ScenarioInputCell.Name property

Obtiene y establece la dirección de la celda de entrada.

```csharp
public string Name { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un escenario
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");

            // Obtener el escenario
            Scenario scenario = scenarios[scenarioIndex];

            // Agregar celdas de entrada al escenario
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(6, 15, "1"); // G16 is row 6, column 15 (0-based)
            inputCells.Add(7, 15, "2"); // H16 is row 7, column 15 (0-based)

            // Obtener las celdas de entrada
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Demostrar el uso de la propiedad Name
            Console.WriteLine("First input cell name: " + inputCell1.Name);
            Console.WriteLine("Second input cell name: " + inputCell2.Name);

            // Verificar que los nombres coincidan con los valores esperados
            if (inputCell1.Name != "G16" || inputCell2.Name != "H16")
            {
                throw new Exception("Input cell names don't match expected values");
            }
        }
    }
}
```

### Ver también

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


