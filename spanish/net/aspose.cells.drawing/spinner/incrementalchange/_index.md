---
title: "Spinner.IncrementalChange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Spinner. Obtiene o establece la cantidad en que la barra de desplazamiento o spinner se incrementa por una línea de desplazamiento"
type: docs
url: /es/net/aspose.cells.drawing/spinner/incrementalchange/
---
## Spinner.IncrementalChange property

Obtiene o establece la cantidad en que la barra de desplazamiento o el spinner se incrementa por desplazamiento de línea.

```csharp
public int IncrementalChange { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un control de spinner
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 100);

            // Establecer propiedades del spinner
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.CurrentValue = 50;
            spinner.IncrementalChange = 5; // Demonstrate IncrementalChange property

            // Verificar y mostrar el valor de IncrementalChange
            Console.WriteLine("Spinner IncrementalChange: " + spinner.IncrementalChange);

            // Modificar y verificar nuevamente
            spinner.IncrementalChange = 10;
            Console.WriteLine("Modified IncrementalChange: " + spinner.IncrementalChange);

            // Guarda el libro de trabajo
            workbook.Save("SpinnerIncrementalChangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


