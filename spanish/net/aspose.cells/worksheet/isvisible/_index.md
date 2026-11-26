---
title: "Worksheet.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Representa si la hoja de cálculo es visible"
type: docs
url: /es/net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

Representa si la hoja de cálculo es visible.

```csharp
public bool IsVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar 3 hojas de cálculo
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Establecer la segunda hoja de cálculo como oculta
            workbook.Worksheets[1].IsVisible = false;
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetVisibilityDemo.xlsx");
            
            // Mostrar estado de visibilidad
            Console.WriteLine("Worksheet Visibility Status:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Console.WriteLine($"{workbook.Worksheets[i].Name}: {(workbook.Worksheets[i].IsVisible ? "Visible" : "Hidden")}");
            }
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


