---
title: "Clase ScenarioInputCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ScenarioInputCell. Representa la celda de entrada para el escenario"
type: docs
url: /es/net/aspose.cells/scenarioinputcell/
---
## ScenarioInputCell class

Representa la celda de entrada para el escenario.

```csharp
public class ScenarioInputCell
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Column](../../aspose.cells/scenarioinputcell/column/) { get; } | Obtiene y establece el índice de columna de la celda de entrada. |
| [IsDeleted](../../aspose.cells/scenarioinputcell/isdeleted/) { get; set; } | Indica si la celda de entrada está eliminada. |
| [Name](../../aspose.cells/scenarioinputcell/name/) { get; } | Obtiene y establece la dirección de la celda de entrada. |
| [Row](../../aspose.cells/scenarioinputcell/row/) { get; } | Obtiene y establece el índice de fila de la celda de entrada. |
| [Value](../../aspose.cells/scenarioinputcell/value/) { get; set; } | Obtiene y establece el valor de la celda de entrada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioInputCellDemo
    {
        public static void ScenarioInputCellExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un escenario a la hoja de cálculo
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Agregar celdas de entrada al escenario
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Adding cell A1 with value 100
            inputCells.Add(1, 1, "200"); // Adding cell B2 with value 200

            // Accediendo a las celdas de entrada
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Mostrando propiedades de las celdas de entrada
            Console.WriteLine($"Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}");
            Console.WriteLine($"Input Cell 2: Row = {inputCell2.Row}, Column = {inputCell2.Column}, Value = {inputCell2.Value}, IsDeleted = {inputCell2.IsDeleted}");

            // Modificar el valor de la primera celda de entrada
            inputCell1.Value = "150";

            // Guarda el libro de trabajo
            workbook.Save("ScenarioInputCellExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


