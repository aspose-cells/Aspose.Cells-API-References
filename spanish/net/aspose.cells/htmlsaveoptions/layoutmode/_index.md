---
title: "HtmlSaveOptions.LayoutMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece el modo de diseño al guardar en HTML. El valor predeterminado es Normal"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/layoutmode/
---
## HtmlSaveOptions.LayoutMode property

Obtiene o establece el modo de diseño al guardar en HTML. El valor predeterminado es Normal

```csharp
public HtmlLayoutMode LayoutMode { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyLayoutModeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Layout Mode Test");

            try
            {
                // Crear instancia de HtmlSaveOptions
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Mostrar el valor actual de LayoutMode
                Console.WriteLine("Current LayoutMode: " + options.LayoutMode);

                // Establecer LayoutMode a Print
                options.LayoutMode = HtmlLayoutMode.Print;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Guardar el libro con modo de diseño Print
                workbook.Save("LayoutModePrint.html", options);

                // Establecer LayoutMode a Normal
                options.LayoutMode = HtmlLayoutMode.Normal;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Guardar el libro con modo de diseño Normal
                workbook.Save("LayoutModeNormal.html", options);

                Console.WriteLine("HTML files saved with different LayoutMode settings.");
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

* enum [HtmlLayoutMode](../../../aspose.cells.rendering/htmllayoutmode/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


