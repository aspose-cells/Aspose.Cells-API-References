---
title: "HtmlLoadOptions.StreamProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlLoadOptions. Obtiene o establece el StreamProviderImportHtmlFile para importar objetos"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/streamprovider/
---
## HtmlLoadOptions.StreamProvider property

Obtiene o establece el StreamProviderImportHtmlFile para importar objetos.

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
    public class HtmlLoadOptionsPropertyStreamProviderDemo : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            // Inicialice el flujo según sea necesario
        }

        public Stream ProvideStream(StreamProviderOptions options)
        {
            // Devuelva un flujo para lectura/escritura
            return File.Open(options.DefaultPath, FileMode.OpenOrCreate, FileAccess.ReadWrite);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Cierre el flujo
            options.Stream.Close();
        }

        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("StreamProvider Demo");

            // Guarde con un StreamProvider personalizado
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            workbook.Save("output.html", saveOptions);

            // Cargue con un StreamProvider personalizado
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("output.html", loadOptions);

            // Verifique los datos cargados
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Ver también

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


