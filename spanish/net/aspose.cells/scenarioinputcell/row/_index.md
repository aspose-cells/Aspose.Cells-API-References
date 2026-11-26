---
title: "ScenarioInputCell.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScenarioInputCell. Obtiene y establece el índice de fila de la celda de entrada"
type: docs
url: /es/net/aspose.cells/scenarioinputcell/row/
---
## ScenarioInputCell.Row property

Obtiene y establece el índice de fila de la celda de entrada.

```csharp
public int Row { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un escenario a la hoja de cálculo
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Agregar celdas de entrada al escenario
            scenario.InputCells.Add(0, 0, "10"); // Cell A1
            scenario.InputCells.Add(1, 1, "20"); // Cell B2

            // Acceder y demostrar la propiedad Row
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at row: {cell1.Row}");

            // Agregar una nueva celda en la fila 2 en lugar de intentar modificar la existente
            worksheet.Cells[2, 0].Value = "30"; // Cell A3
            scenario.InputCells.Add(2, 0, "30");
            Console.WriteLine($"New input cell added at row: {scenario.InputCells[2].Row}");

            // Guarda el libro de trabajo
            workbook.Save("ScenarioInputCellRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


