---
title: "ImageSaveOptions.StreamProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageSaveOptions. Obtiene o establece el IStreamProvider para exportar objetos"
type: docs
url: /es/net/aspose.cells/imagesaveoptions/streamprovider/
---
## ImageSaveOptions.StreamProvider property

Obtiene o establece el IStreamProvider para exportar objetos.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Observaciones

Si se guarda como Tiff, esta propiedad se ignora. De lo contrario, si se deben guardar más de una imagen, escribiremos las demás imágenes mediante esta. Para uso avanzado, por favor use [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) o [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomStreamProvider : IStreamProvider
    {
        private int m_count = 0;

        public void InitStream(StreamProviderOptions options)
        {
            m_count++;
        }

        public Stream GetStream(StreamProviderOptions options)
        {
            return new FileStream(options.DefaultPath + m_count + ".png", FileMode.Create);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementación cuando no se proporciona una secuencia
        }

        public void CloseStream(StreamProviderOptions options, Stream stream)
        {
            stream.Dispose();
        }
    }

    public class ImageSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test StreamProvider");

            // Establecer opciones de guardado con un proveedor de secuencia personalizado
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            saveOptions.StreamProvider = new CustomStreamProvider();

            // Guardar con proveedor de secuencia
            workbook.Save("output.png", saveOptions);
        }
    }
}
```

### Ver también

* interface [IStreamProvider](../../istreamprovider/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


