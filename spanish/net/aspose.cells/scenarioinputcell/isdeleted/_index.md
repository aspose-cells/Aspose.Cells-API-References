---
title: "ScenarioInputCell.IsDeleted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScenarioInputCell. Indica si la celda de entrada está eliminada"
type: docs
url: /es/net/aspose.cells/scenarioinputcell/isdeleted/
---
## ScenarioInputCell.IsDeleted property

Indica si la celda de entrada está eliminada.

```csharp
public bool IsDeleted { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un escenario
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Agregar celdas de entrada
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100");
            inputCells.Add(1, 1, "200");

            // Acceder y mostrar celdas de entrada
            ScenarioInputCell cell1 = inputCells[0];
            Console.WriteLine($"Cell A1 - Value: {cell1.Value}, IsDeleted: {cell1.IsDeleted}");

            // Eliminar la primera celda de entrada
            cell1.IsDeleted = true;
            Console.WriteLine($"After deletion - Cell A1 IsDeleted: {cell1.IsDeleted}");

            // Guarda el libro de trabajo
            workbook.Save("ScenarioWithDeletedCell.xlsx");
        }
    }
}
```

### Ver también

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


