---
title: "Spinner.Min"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Spinner. Obtiene o establece el valor mínimo de una barra de desplazamiento o rango de spinner"
type: docs
url: /es/net/aspose.cells.drawing/spinner/min/
---
## Spinner.Min property

Obtiene o establece el valor mínimo del rango de una barra de desplazamiento o spinner.

```csharp
public int Min { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMinDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control de spinner con dimensiones adecuadas
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 1, 1, 1, 100, 20);

            // Establecer propiedades del spinner, incluido Min
            spinner.Min = 10;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 15;

            // Verificar y mostrar la propiedad Min
            Console.WriteLine("Spinner Min Value: " + spinner.Min);

            // Guarda el libro de trabajo
            workbook.Save("SpinnerPropertyMinDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


