---
title: "HtmlLoadOptions.AttachedFilesDirectory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlLoadOptions. El directorio donde se guardarán los archivos adjuntos"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/attachedfilesdirectory/
---
## HtmlLoadOptions.AttachedFilesDirectory property

El directorio donde se guardarán los archivos adjuntos.

```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad HtmlLoadOptions.StreamProvider. Esta propiedad será eliminada 12 meses después desde diciembre de 2014. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // Crea una instancia de HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Establecer el directorio para los archivos adjuntos
            options.AttachedFilesDirectory = "C:\\AttachedFiles";

            // Cargar un archivo HTML en un Libro de trabajo usando las opciones especificadas
            Workbook workbook = new Workbook("input.html", options);

            // Guarda el libro de trabajo en un archivo Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


