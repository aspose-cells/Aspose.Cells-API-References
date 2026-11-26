---
title: "LoadOptions.IgnoreUselessShapes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Indica si se ignoran formas inútiles"
type: docs
url: /es/net/aspose.cells/loadoptions/ignoreuselessshapes/
---
## LoadOptions.IgnoreUselessShapes property

Indica si se ignoran formas inútiles.

```csharp
public bool IgnoreUselessShapes { get; set; }
```

### Observaciones

Solo funciona para archivos xlsx, xlsb y xlsm. Hay muchas formas idénticas superpuestas que son inútiles en algunos archivos; podemos ignorarlas al cargar los archivos.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreUselessShapesDemo
    {
        public static void Run()
        {
            // Crear LoadOptions y establecer IgnoreUselessShapes a true
            LoadOptions options = new LoadOptions();
            options.IgnoreUselessShapes = true;

            // Cargue el libro de trabajo con las opciones
            Workbook workbook = new Workbook("example.xlsx", options);

            // Mostrar el recuento de formas en la primera hoja de cálculo
            Console.WriteLine("Shapes count: " + workbook.Worksheets[0].Shapes.Count);
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


