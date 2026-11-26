---
title: "Spinner.Shadow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Spinner. Indica si la forma tiene sombreado 3D"
type: docs
url: /es/net/aspose.cells.drawing/spinner/shadow/
---
## Spinner.Shadow property

Indica si la forma tiene sombreado 3-D.

```csharp
public bool Shadow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyShadowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añadir un spinner a la hoja de cálculo
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);

            // Establecer propiedades del spinner
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 50;

            // Demostrar la propiedad Shadow
            spinner.Shadow = true; // Enable 3D shadow effect
            Console.WriteLine("Spinner shadow enabled: " + spinner.Shadow);

            // Guarda el libro de trabajo
            workbook.Save("SpinnerShadowDemo.xlsx");

            // Cargar el libro de trabajo guardado para verificar la propiedad de sombra
            Workbook verifyWorkbook = new Workbook("SpinnerShadowDemo.xlsx");
            Spinner verifySpinner = (Spinner)verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Verified spinner shadow: " + verifySpinner.Shadow);
        }
    }
}
```

### Ver también

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


