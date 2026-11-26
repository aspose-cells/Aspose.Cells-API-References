---
title: "ScenarioInputCell.Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScenarioInputCell. Obtiene y establece el índice de columna de la celda de entrada"
type: docs
url: /es/net/aspose.cells/scenarioinputcell/column/
---
## ScenarioInputCell.Column property

Obtiene y establece el índice de columna de la celda de entrada.

```csharp
public int Column { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyColumnDemo
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

            // Acceder y demostrar la propiedad Column
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at column: {cell1.Column}");

            // Dado que Column es de solo lectura, necesitamos eliminar y volver a agregar para cambiar la columna
            string value = cell1.Value;
            scenario.InputCells.RemoveAt(0);
            scenario.InputCells.Add(0, 2, value); // Add at new column 2 with same value

            // Verificar el cambio
            cell1 = scenario.InputCells[0];
            Console.WriteLine($"Modified first input cell column to: {cell1.Column}");

            // Guarda el libro de trabajo
            workbook.Save("ScenarioInputCellColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


