---
title: "Interfaz IStreamProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Interfaz Aspose.Cells.IStreamProvider. Representa el proveedor de flujo exportado"
type: docs
url: /es/net/aspose.cells/istreamprovider/
---
## IStreamProvider interface

Representa el proveedor de flujo exportado.

```csharp
public interface IStreamProvider
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CloseStream](../../aspose.cells/istreamprovider/closestream/)(StreamProviderOptions) | Cierra el flujo. |
| [InitStream](../../aspose.cells/istreamprovider/initstream/)(StreamProviderOptions) | Obtiene el flujo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderDemo : IStreamProvider
    {
        // Implementando el método InitStream
        public void InitStream(StreamProviderOptions options)
        {
            string outputDir = "/test/";
            string path = outputDir + Path.GetFileName(options.DefaultPath);
            options.CustomPath = path;
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
        }

        // Implementando el método CloseStream
        public void CloseStream(StreamProviderOptions options)
        {
            // Cierra el flujo si no es nulo
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }

        public static void IStreamProviderExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer algunos datos en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Hello World");

            // Cree HtmlSaveOptions y establezca el StreamProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new IStreamProviderDemo();

            // Guarde el libro de trabajo en formato HTML
            workbook.Save("IStreamProviderExample.html", saveOptions);

            // Cargue el libro de trabajo desde formato HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new IStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("IStreamProviderExample.html", loadOptions);

            // Muestre los datos cargados
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }

}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


