---
title: "Spinner.CurrentValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Spinner. Obtiene o establece el valor actual"
type: docs
url: /es/net/aspose.cells.drawing/spinner/currentvalue/
---
## Spinner.CurrentValue property

Obtiene o establece el valor actual.

```csharp
public int CurrentValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control de spinner
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Spinner, 1, 1, 0, 0, 20, 20);
            Spinner spinner = (Spinner)shape;

            // Establecer propiedades del spinner
            spinner.LinkedCell = "A1";
            spinner.Min = 1;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 10; // Using CurrentValue property directly

            // Verificar y mostrar el valor actual
            Console.WriteLine("Spinner CurrentValue: " + spinner.CurrentValue);

            // Guarda el libro de trabajo
            workbook.Save("SpinnerDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


