---
title: "Worksheet.Scenarios"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene la colección de Scenario"
type: docs
url: /es/net/aspose.cells/worksheet/scenarios/
---
## Worksheet.Scenarios property

Obtiene la colección de [`Scenario`](../../scenario/).

```csharp
public ScenarioCollection Scenarios { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyScenariosDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Agregar escenarios
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex1 = scenarios.Add("Scenario1");
            Scenario scenario1 = scenarios[scenarioIndex1];
            scenario1.Comment = "First test scenario";
            
            int scenarioIndex2 = scenarios.Add("Scenario2");
            Scenario scenario2 = scenarios[scenarioIndex2];
            scenario2.Comment = "Second test scenario";
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetPropertyScenariosDemo.xlsx");
            
            // Borrar escenarios y guardar de nuevo
            scenarios.Clear();
            workbook.Save("WorksheetPropertyScenariosDemo_Cleared.xlsx");
        }
    }
}
```

### Ver también

* class [ScenarioCollection](../../scenariocollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


