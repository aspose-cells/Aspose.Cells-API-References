---
title: "Enumeración HtmlLayoutMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Rendering.HtmlLayoutMode. Representa el modo de diseño para la renderización HTML"
type: docs
url: /es/net/aspose.cells.rendering/htmllayoutmode/
---
## HtmlLayoutMode enumeration

Representa el modo de diseño para el renderizado HTML.

```csharp
public enum HtmlLayoutMode
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Normal | `0` | Renderiza contenido como MS Excel. |
| Print | `1` | Renderiza contenido en modo de diseño de impresión. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlLayoutModeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar algunos datos de ejemplo a la hoja de cálculo
                worksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
                worksheet.Cells["A2"].PutValue("This demonstrates HtmlLayoutMode");

                // Crea HtmlSaveOptions y establece el modo de diseño a Normal
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.LayoutMode = HtmlLayoutMode.Normal;

                // Guarda el libro de trabajo con modo de diseño normal
                workbook.Save("NormalLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Normal layout mode.");

                // Cambia el modo de diseño a Imprimir
                saveOptions.LayoutMode = HtmlLayoutMode.Print;

                // Guarda el libro de trabajo con modo de diseño de impresión
                workbook.Save("PrintLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Print layout mode.");

                // Mostrar los valores del enum
                Console.WriteLine($"Normal mode value: {HtmlLayoutMode.Normal}");
                Console.WriteLine($"Print mode value: {HtmlLayoutMode.Print}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlLayoutMode: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


