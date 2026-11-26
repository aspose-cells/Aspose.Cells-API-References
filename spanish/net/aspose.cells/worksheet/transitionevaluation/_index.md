---
title: "Worksheet.TransitionEvaluation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Indica si la opción de compatibilidad Lotus de Evaluación de Fórmula de Transición está habilitada"
type: docs
url: /es/net/aspose.cells/worksheet/transitionevaluation/
---
## Worksheet.TransitionEvaluation property

Indica si la opción de Evaluación de Fórmula de Transición (compatibilidad Lotus) está habilitada.

```csharp
public bool TransitionEvaluation { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEvaluationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la propiedad TransitionEvaluation
            worksheet.TransitionEvaluation = true;
            
            // Mostrar el valor de la propiedad
            Console.WriteLine("TransitionEvaluation: " + worksheet.TransitionEvaluation);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Cargar el libro de trabajo guardado para verificar la propiedad
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("Loaded TransitionEvaluation: " + loadedWorksheet.TransitionEvaluation);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


