---
title: "Spinner.IsHorizontal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Spinner. Indica si se trata de una barra de desplazamiento horizontal"
type: docs
url: /es/net/aspose.cells.drawing/spinner/ishorizontal/
---
## Spinner.IsHorizontal property

Indica si esta es una barra de desplazamiento horizontal.

```csharp
public bool IsHorizontal { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SpinnerPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Agregar una forma de spinner a la hoja de cálculo
                Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);
                
                // Establecer propiedades del spinner
                spinner.Min = 0;
                spinner.Max = 100;
                spinner.IncrementalChange = 5;
                spinner.CurrentValue = 50;
                
                // Demostrar la propiedad IsHorizontal (lectura y escritura)
                Console.WriteLine("Initial IsHorizontal value: " + spinner.IsHorizontal);
                
                // Alternar la orientación
                spinner.IsHorizontal = !spinner.IsHorizontal;
                Console.WriteLine("Modified IsHorizontal value: " + spinner.IsHorizontal);
                
                // Guarda el libro de trabajo
                workbook.Save("SpinnerIsHorizontalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


