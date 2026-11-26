---
title: "Worksheet.GetSelectedAreas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Obtiene los rangos de celdas seleccionados en la hoja de cálculo del diseñador"
type: docs
url: /es/net/aspose.cells/worksheet/getselectedareas/
---
## Worksheet.GetSelectedAreas method

Obtiene los rangos de celdas seleccionados en la hoja de cálculo del diseñador.

```csharp
public Range[] GetSelectedAreas()
```

### Valor de retorno

Devuelve todos los rangos seleccionados.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetSelectedAreasDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Seleccionar varios rangos
            worksheet.SelectRange(0, 0, 2, 2, false); // First range (A1:C3)
            worksheet.SelectRange(4, 4, 6, 6, false); // Second range (E5:G7)
            
            // Obtener áreas seleccionadas
            Aspose.Cells.Range[] selectedAreas = worksheet.GetSelectedAreas();
            
            // Mostrar información sobre las áreas seleccionadas
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            for (int i = 0; i < selectedAreas.Length; i++)
            {
                Console.WriteLine($"Area {i + 1}: {selectedAreas[i].Address}");
            }
            
            // Borrar selecciones y seleccionar un solo rango
            worksheet.SelectRange(1, 1, 3, 3, true); // New single selection (B2:D4)
            
            // Obtener el área seleccionada única
            selectedAreas = worksheet.GetSelectedAreas();
            Console.WriteLine("\nAfter single selection:");
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            Console.WriteLine("Selected area: " + selectedAreas[0].Address);
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


