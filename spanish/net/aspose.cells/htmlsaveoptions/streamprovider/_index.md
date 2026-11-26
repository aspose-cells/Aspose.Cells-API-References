---
title: "HtmlSaveOptions.StreamProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "HtmlSaveOptions propiedad. Obtiene o establece el IStreamProvider para exportar objetos"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/streamprovider/
---
## HtmlSaveOptions.StreamProvider property

Obtiene o establece el IStreamProvider para exportar objetos.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Crear un directorio temporal para la salida
            string outputDir = Path.Combine(Path.GetTempPath(), "AsposeStreamProviderDemo");
            Directory.CreateDirectory(outputDir);

            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("StreamProvider Demo");

            // Configurar opciones de guardado HTML con un proveedor de flujo personalizado
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.StreamProvider = new ExportStreamProvider(outputDir);

            // Guarda el libro de trabajo como HTML
            string outputPath = Path.Combine(outputDir, "output.html");
            workbook.Save(outputPath, options);

            Console.WriteLine($"File saved with StreamProvider to: {outputPath}");
        }
    }

    public class ExportStreamProvider : IStreamProvider
    {
        private readonly string _outputDirectory;

        public ExportStreamProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Inicialización si es necesario
        }

        public Stream GetStream(StreamProviderOptions options)
        {
            string filePath = Path.Combine(_outputDirectory, options.CustomPath);
            return new FileStream(filePath, FileMode.Create);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementación según lo requiera la interfaz
        }
    }
}
```

### Ver también

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


