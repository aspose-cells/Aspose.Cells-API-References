---
title: "PageStartSavingArgs.IsToOutput"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageStartSavingArgs. Obtiene o establece un valor que indica si la página debe ser salida. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells.rendering/pagestartsavingargs/istooutput/
---
## PageStartSavingArgs.IsToOutput property

Obtiene o establece un valor que indica si la página debe ser exportada. El valor predeterminado es true.

```csharp
public bool IsToOutput { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageStartSavingArgsPropertyIsToOutputDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pobla datos para crear múltiples páginas
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
                // Corregido: Acceder a la altura de la fila a través de la colección Rows de la hoja de cálculo
                worksheet.Cells.Rows[i].Height = 50;
            }

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            workbook.Save("PageOutputDemo.pdf", saveOptions);
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Leer el valor actual
                Console.WriteLine($"Page {args.PageIndex + 1} - Initial IsToOutput: {args.IsToOutput}");

                // Omitir cada página con número par (numeración basada en 1)
                if ((args.PageIndex + 1) % 2 == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine($"Disabling output for page {args.PageIndex + 1}");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Implementación no requerida para esta demostración
            }
        }
    }
}
```

### Ver también

* class [PageStartSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


