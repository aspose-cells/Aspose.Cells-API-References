---
title: "HtmlSaveOptions.EmbeddedFontType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece el tipo de incrustación de archivo de fuente en el archivo html. El valor predeterminado es None, lo que indica que no se incrustará ninguna fuente en html."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/embeddedfonttype/
---
## HtmlSaveOptions.EmbeddedFontType property

Obtiene o establece el tipo de incrustación de archivos de fuente en el archivo html. El valor predeterminado es None, lo que indica que no se incrustará ninguna fuente en html.

```csharp
public HtmlEmbeddedFontType EmbeddedFontType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Text with Font");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);

            try
            {
                // Crear opciones de guardado HTML
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Mostrar el valor predeterminado de EmbeddedFontType
                Console.WriteLine("Default EmbeddedFontType: " + options.EmbeddedFontType);

                // Establecer EmbeddedFontType a Woff
                options.EmbeddedFontType = HtmlEmbeddedFontType.Woff;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Guardar el libro de trabajo con incrustación de fuente WOFF
                workbook.Save("EmbeddedFontType_Woff.html", options);

                // Restablecer a None
                options.EmbeddedFontType = HtmlEmbeddedFontType.None;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Guardar el libro de trabajo sin incrustar fuentes
                workbook.Save("EmbeddedFontType_None.html", options);

                Console.WriteLine("EmbeddedFontType demonstration completed successfully.");
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

* enum [HtmlEmbeddedFontType](../../../aspose.cells.rendering/htmlembeddedfonttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


