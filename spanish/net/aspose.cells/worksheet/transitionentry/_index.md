---
title: "Worksheet.TransitionEntry"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Indica si la opción de compatibilidad Lotus de Transition Formula Entry está habilitada"
type: docs
url: /es/net/aspose.cells/worksheet/transitionentry/
---
## Worksheet.TransitionEntry property

Indica si la opción de Entrada de Fórmula de Transición (compatibilidad Lotus) está habilitada.

```csharp
public bool TransitionEntry { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEntryDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la propiedad TransitionEntry
            worksheet.TransitionEntry = true;
            
            // Mostrar el valor de TransitionEntry
            Console.WriteLine("TransitionEntry: " + worksheet.TransitionEntry);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Cargar el libro de trabajo guardado para verificar la propiedad
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Mostrar el valor de TransitionEntry cargado
            Console.WriteLine("Loaded TransitionEntry: " + loadedWorksheet.TransitionEntry);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


