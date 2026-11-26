---
title: "HtmlSaveOptions.SaveAsSingleFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se guarda el HTML como un solo archivo. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/saveassinglefile/
---
## HtmlSaveOptions.SaveAsSingleFile property

Indica si se guarda el HTML como un solo archivo. El valor predeterminado es false.

```csharp
public bool SaveAsSingleFile { get; set; }
```

### Observaciones

Si hay varias hojas de cálculo u otros recursos necesarios, como imágenes, en el libro, normalmente esas hojas y recursos deben guardarse en archivos separados. En algunos escenarios, el usuario puede necesitar obtener un solo archivo resultante, por ejemplo para facilitar la transferencia. En ese caso, el usuario puede establecer esta propiedad como true.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertySaveAsSingleFileDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Inicializar opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.SaveAsSingleFile = true;
            saveOptions.ExportPageHeaders = true;
            
            // Guardar el libro como un solo archivo HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            // Verificar que el archivo de salida exista
            if (File.Exists(outputPath))
            {
                Console.WriteLine("HTML saved as single file successfully.");
            }
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


