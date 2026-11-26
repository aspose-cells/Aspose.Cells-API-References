---
title: "HtmlSaveOptions.IsExpImageToTempDir"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan archivos de imagen al directorio temporal. Solo para guardar en flujo html"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/isexpimagetotempdir/
---
## HtmlSaveOptions.IsExpImageToTempDir property

Indica si se exportan los archivos de imagen a un directorio temporal. Solo para guardar en flujo HTML.

```csharp
public bool IsExpImageToTempDir { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsExpImageToTempDirDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con una imagen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una imagen de ejemplo a la hoja de cálculo
            worksheet.Pictures.Add(0, 0, "https://www.aspose.com/templates/aspose/App_Themes/V3/images/cells/header/aspose_cells-for-net.png");

            // Establecer opciones de guardado HTML con IsExpImageToTempDir habilitado
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.IsExpImageToTempDir = true;
            options.ExportImagesAsBase64 = false; // Ensure images are exported as separate files

            // Guarda el libro de trabajo como HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML saved with images exported to temp directory.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


