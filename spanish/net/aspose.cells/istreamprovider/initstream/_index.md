---
title: "IStreamProvider.InitStream"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IStreamProvider. Obtiene el flujo"
type: docs
url: /es/net/aspose.cells/istreamprovider/initstream/
---
## IStreamProvider.InitStream method

Obtiene el flujo.

```csharp
public void InitStream(StreamProviderOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | StreamProviderOptions |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo : IStreamProvider
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear una instancia de la clase de demostración que implementa IStreamProvider
            var streamProvider = new IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo();
            
            // Preparar StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "custom_path",
                Stream = new MemoryStream()
            };

            try
            {
                // Llamar al método InitStream con el parámetro StreamProviderOptions
                streamProvider.InitStream(options);
                
                Console.WriteLine("InitStream method executed successfully with StreamProviderOptions parameter");
                
                // Demostrar el efecto - en este caso solo estamos mostrando que el stream está inicializado
                Console.WriteLine($"Stream initialized: {options.Stream != null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitStream method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("MethodInitStreamWithStreamProviderOptionsDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Implementación de InitStream
            Console.WriteLine($"Initializing stream with ResourceLoadingType: {options.ResourceLoadingType}");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementación de CloseStream
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }
    }
}
```

### Ver también

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


