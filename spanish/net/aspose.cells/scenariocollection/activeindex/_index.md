---
title: "ScenarioCollection.ActiveIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScenarioCollection. Obtiene y establece qué escenario está seleccionado"
type: docs
url: /es/net/aspose.cells/scenariocollection/activeindex/
---
## ScenarioCollection.ActiveIndex property

Obtiene y establece cuál escenario está seleccionado.

```csharp
public int ActiveIndex { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyActiveIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");
            
            scenarios.ActiveIndex = scenarioIndex;
            
            Console.WriteLine($"Active scenario index set to: {scenarios.ActiveIndex}");
            
            workbook.Save("ScenarioActiveIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


