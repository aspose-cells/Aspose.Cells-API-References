---
title: "StreamProviderOptions.CustomPath"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StreamProviderOptions. La ruta personalizada del usuario (pathURL) guardada en el archivo HTML generado para la fuente referenciada. Si no es definida por el usuario, se usará DefaultPath. Por ejemplo, los datos de la hoja serán guardados por el usuario en d/sheet001.htm; la URL utilizada en el archivo HTML principal debe ser d/sheet001.htm u otra ruta relativa válida que pueda ser accedida por el archivo HTML principal."
type: docs
url: /es/net/aspose.cells/streamprovideroptions/custompath/
---
## StreamProviderOptions.CustomPath property

La ruta personalizada del usuario (URL) guardada en el archivo HTML generado para la fuente referenciada. Si no es definida por el usuario, se utilizará DefaultPath. Por ejemplo, los datos de la hoja serán guardados por el usuario en d:/sheet001.htm, la URL utilizada en el archivo HTML principal debería ser "d:/sheet001.htm" u otra ruta relativa válida que pueda ser accedida por el archivo HTML principal.

```csharp
public string CustomPath { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyCustomPathDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Configurar opciones de guardado HTML con un proveedor de flujo personalizado
            string outputDir = "output";
            Directory.CreateDirectory(outputDir);
            
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            
            // Crear proveedor de flujo personalizado con CustomPath
            HtmlWithExternalResourcesProvider streamProvider = new HtmlWithExternalResourcesProvider(outputDir);
            streamProvider.streamProviderOptions.CustomPath = "resources";
            options.StreamProvider = streamProvider;

            // Guarda el libro de trabajo
            string outputFile = Path.Combine(outputDir, "output.html");
            workbook.Save(outputFile, options);

            // Verificar que se utilizó la ruta personalizada
            string resourcePath = Path.Combine(outputDir, streamProvider.streamProviderOptions.CustomPath);
            Console.WriteLine($"Resources should be saved to: {resourcePath}");
        }
    }

    // Implementación simplificada del proveedor de flujo personalizado
    public class HtmlWithExternalResourcesProvider : IStreamProvider
    {
        public StreamProviderOptions streamProviderOptions = new StreamProviderOptions();
        public string _outputDirectory;

        public HtmlWithExternalResourcesProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // La implementación iría aquí
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // La implementación iría aquí
        }
    }
}
```

### Ver también

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


