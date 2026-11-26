---
title: "ScenarioCollection.LastSelected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScenarioCollection. Indica qué escenario fue seleccionado por última vez por el usuario para ejecutarse/mostrarse"
type: docs
url: /es/net/aspose.cells/scenariocollection/lastselected/
---
## ScenarioCollection.LastSelected property

Indica cuál escenario fue seleccionado por última vez por el usuario para ejecutarse/mostrarse.

```csharp
public int LastSelected { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyLastSelectedDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar escenarios
            ScenarioCollection scenarios = worksheet.Scenarios;
            scenarios.Add("Scenario1");
            scenarios.Add("Scenario2");

            // Establezca el escenario activo y el índice seleccionado por última vez
            scenarios.ActiveIndex = 1;
            scenarios.LastSelected = 1;

            // Verifique y demuestre la propiedad LastSelected
            Console.WriteLine("Total scenarios: " + scenarios.Count);
            Console.WriteLine("Active scenario index: " + scenarios.ActiveIndex);
            Console.WriteLine("Last selected scenario index: " + scenarios.LastSelected);

            // Modifique el índice seleccionado por última vez
            scenarios.LastSelected = 0;
            Console.WriteLine("Updated last selected scenario index: " + scenarios.LastSelected);
        }
    }
}
```

### Ver también

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


