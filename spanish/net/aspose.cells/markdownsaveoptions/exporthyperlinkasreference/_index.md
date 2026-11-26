---
title: "MarkdownSaveOptions.ExportHyperlinkAsReference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Indica si se debe exportar el hipervínculo usando definiciones de referencia en lugar de formato en línea. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/exporthyperlinkasreference/
---
## MarkdownSaveOptions.ExportHyperlinkAsReference property

Indica si se debe exportar el hipervínculo usando definiciones de referencia en lugar del formato en línea. El valor predeterminado es falso.

```csharp
public bool ExportHyperlinkAsReference { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportHyperlinkAsReferenceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Colocar un texto de ejemplo en una celda
            sheet.Cells["A1"].PutValue("Visit Aspose");

            // Agregar un hipervínculo a la celda (A1)
            // Parámetros: firstRow, firstColumn, totalRows, totalColumns, hyperlink
            sheet.Hyperlinks.Add(0, 0, 1, 1, "https://www.aspose.com");

            // Inicializar opciones de guardado Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Acceder directamente a la propiedad ExportHyperlinkAsReference (solo lectura en esta demostración)
                Console.WriteLine("ExportHyperlinkAsReference value: " + saveOptions.ExportHyperlinkAsReference);

                // Guardar el libro de trabajo como markdown; la propiedad (si es true) afectará cómo se exportan los hipervínculos
                workbook.Save("ExportHyperlinkAsReferenceDemo.md", saveOptions);
                Console.WriteLine("Workbook saved as markdown.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


