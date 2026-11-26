---
title: "MarkdownSaveOptions.StreamProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Obtiene o establece el IStreamProvider para exportar objetos. Si es nulo, los objetos exportados se guardarán en el mismo directorio que el archivo de salida"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/streamprovider/
---
## MarkdownSaveOptions.StreamProvider property

Obtiene o establece el IStreamProvider para exportar objetos. Si `null`, los objetos exportados se guardarán en el mismo directorio que el archivo de salida.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MarkdownSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = "Hello";
            worksheet.Cells["B1"].Value = "World";

            try
            {
                // Crear una instancia de MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Mostrar el valor actual de StreamProvider (null por defecto)
                Console.WriteLine("Current StreamProvider: " + (saveOptions.StreamProvider == null ? "null" : "set"));

                // Crear una implementación personalizada de StreamProvider
                CustomStreamProvider streamProvider = new CustomStreamProvider();
                saveOptions.StreamProvider = streamProvider;

                // Mostrar el valor actualizado de StreamProvider
                Console.WriteLine("Updated StreamProvider: " + (saveOptions.StreamProvider != null ? "set" : "null"));

                // Guardar el libro de trabajo con el StreamProvider personalizado
                workbook.Save("StreamProviderDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved with custom StreamProvider.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    // Implementación personalizada de IStreamProvider
    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            Console.WriteLine("Initializing stream");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            Console.WriteLine("Closing stream");
        }
    }
}
```

### Ver también

* interface [IStreamProvider](../../istreamprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


