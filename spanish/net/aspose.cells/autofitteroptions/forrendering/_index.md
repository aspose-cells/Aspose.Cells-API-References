---
title: "AutoFitterOptions.ForRendering"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFitterOptions. Indica si se ajusta para propósitos de renderizado"
type: docs
url: /es/net/aspose.cells/autofitteroptions/forrendering/
---
## AutoFitterOptions.ForRendering property

Indica si es adecuado para fines de renderizado.

```csharp
public bool ForRendering { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyForRenderingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer datos de ejemplo con texto largo
            worksheet.Cells["A1"].PutValue("This is a long text that needs auto-fitting for rendering purposes.");
            
            // Crear AutoFitterOptions y establecer ForRendering a true
            AutoFitterOptions options = new AutoFitterOptions();
            options.ForRendering = true;

            // Ajustar automáticamente la fila con consideraciones de renderizado
            worksheet.AutoFitRows(0, 0, options);

            // Mostrar la altura resultante de la fila en píxeles
            Console.WriteLine("Row height after auto-fitting (pixels): " + worksheet.Cells.GetRowHeightPixel(0));
        }
    }
}
```

### Ver también

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


