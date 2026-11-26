---
title: "Spinner.Max"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Spinner. Obtiene o establece el valor máximo de una barra de desplazamiento o del rango del spinner"
type: docs
url: /es/net/aspose.cells.drawing/spinner/max/
---
## Spinner.Max property

Obtiene o establece el valor máximo del rango de una barra de desplazamiento o spinner.

```csharp
public int Max { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMaxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Spinner spinner = sheet.Shapes.AddSpinner(1, 1, 0, 0, 100, 100);
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;

            Console.WriteLine($"Spinner Max Value: {spinner.Max}");
        }
    }
}
```

### Ver también

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


