---
title: "HtmlSaveOptions.AttachedFilesDirectory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. El directorio donde se guardarán los archivos adjuntos. Solo para guardar en flujo html"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/attachedfilesdirectory/
---
## HtmlSaveOptions.AttachedFilesDirectory property

El directorio donde se guardarán los archivos adjuntos. Solo para guardar en un flujo html.

```csharp
public string AttachedFilesDirectory { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // Crear un directorio temporal para la demostración
            string tempDir = Path.Combine(Path.GetTempPath(), "AsposeAttachedFilesDemo");
            Directory.CreateDirectory(tempDir);

            try
            {
                // Crear un libro de trabajo de ejemplo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Hello World");

                // Establecer las opciones de guardado HTML con AttachedFilesDirectory
                HtmlSaveOptions options = new HtmlSaveOptions();
                options.AttachedFilesDirectory = tempDir;

                // Guarda el libro de trabajo como HTML
                string outputPath = Path.Combine(tempDir, "output.html");
                workbook.Save(outputPath, options);

                // Verificar que los archivos adjuntos fueron creados
                Console.WriteLine("HTML saved with attached files in: " + tempDir);
                Console.WriteLine("Attached files exist: " + 
                    File.Exists(Path.Combine(tempDir, "sheet001.htm")));
            }
            finally
            {
                // Limpiar
                Directory.Delete(tempDir, true);
            }
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


