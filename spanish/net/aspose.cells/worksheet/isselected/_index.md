---
title: "Worksheet.IsSelected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Indica si esta hoja de cálculo está seleccionada cuando se abre el libro de trabajo"
type: docs
url: /es/net/aspose.cells/worksheet/isselected/
---
## Worksheet.IsSelected property

Indica si esta hoja de cálculo está seleccionada cuando se abre el libro de trabajo.

```csharp
public bool IsSelected { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsSelectedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una segunda hoja de cálculo
            workbook.Worksheets.Add("Sheet2");
            
            // Obtener la primera hoja de cálculo
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "FirstSheet";
            
            // Obtener la segunda hoja de cálculo
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet2.Name = "SecondSheet";
            
            // Demostrar la propiedad IsSelected
            Console.WriteLine("Before selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Seleccionar la segunda hoja de cálculo
            worksheet2.IsSelected = true;
            workbook.Worksheets.ActiveSheetIndex = worksheet2.Index;
            
            Console.WriteLine("\nAfter selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetSelectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


