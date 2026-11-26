---
title: "HtmlSaveOptions.AttachedFilesUrlPrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Especifica el prefijo Url de los archivos adjuntos, como imágenes, en el archivo HTML. Solo para guardar en un flujo HTML"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/attachedfilesurlprefix/
---
## HtmlSaveOptions.AttachedFilesUrlPrefix property

Especifique el prefijo Url de los archivos adjuntos, como imágenes, en el archivo html. Solo para guardar en un flujo html.

```csharp
public string AttachedFilesUrlPrefix { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesUrlPrefixDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // Establecer las opciones de guardado HTML con AttachedFilesUrlPrefix
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AttachedFilesUrlPrefix = "www.aspose.com";

            // Guardar el libro de trabajo con opciones HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with AttachedFilesUrlPrefix: " + saveOptions.AttachedFilesUrlPrefix);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


