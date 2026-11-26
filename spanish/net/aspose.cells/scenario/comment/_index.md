---
title: "Scenario.Comment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Scenario. Obtiene y establece el comentario del escenario"
type: docs
url: /es/net/aspose.cells/scenario/comment/
---
## Scenario.Comment property

Obtiene y establece el comentario del escenario.

```csharp
public string Comment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyCommentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una colección de escenarios
            ScenarioCollection scenarios = worksheet.Scenarios;
            
            // Agregar un escenario
            int index = scenarios.Add("test");
            Scenario scenario = scenarios[index];
            
            // Establecer propiedades del escenario
            scenario.IsLocked = true;
            scenario.Comment = "创建者 Simon 日期 " + DateTime.Now.ToShortDateString();
            
            // Agregar celdas de entrada al escenario usando referencias de celda y valores
            scenario.InputCells.Add(0, 6, "1");  // G16 (row 0, column 6)
            scenario.InputCells.Add(0, 0, "100"); // A1
            scenario.InputCells.Add(1, 1, "200"); // B2
            scenario.InputCells.Add(2, 2, "300"); // C3

            // Mostrar comentario del escenario
            Console.WriteLine("Scenario Comment: " + scenario.Comment);
            
            // Guarda el libro de trabajo
            workbook.Save("ScenarioCommentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


