---
title: "IStreamProvider.CloseStream"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IStreamProvider. Cierra el stream"
type: docs
url: /es/net/aspose.cells/istreamprovider/closestream/
---
## IStreamProvider.CloseStream method

Cierra el flujo.

```csharp
public void CloseStream(StreamProviderOptions options)
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

    public class IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo : IStreamProvider
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear una instancia de la clase de demostración que implementa IStreamProvider
            var streamProvider = new IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo();
            
            // Crear StreamProviderOptions
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "output_files/sheet001.htm",
                Stream = new MemoryStream()
            };

            try
            {
                // Llamar al método CloseStream
                streamProvider.CloseStream(options);
                
                Console.WriteLine("CloseStream method executed successfully with StreamProviderOptions");
                
                // Demostrar el efecto - en un escenario real, esto cerraría el stream
                Console.WriteLine($"Stream closed status: {options.Stream == null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CloseStream method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("IStreamProviderCloseStreamDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Implementación requerida por la interfaz
        }

        public void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
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


