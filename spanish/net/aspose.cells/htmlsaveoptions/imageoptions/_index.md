---
title: "HtmlSaveOptions.ImageOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Obtén el objeto ImageOrPrintOptions antes de exportar"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/imageoptions/
---
## HtmlSaveOptions.ImageOptions property

Obtenga el objeto ImageOrPrintOptions antes de exportar

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Establecer opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Configurar opciones de imagen
            ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;
            imageOptions.ImageType = ImageType.Svg;
            imageOptions.HorizontalResolution = 300;
            imageOptions.VerticalResolution = 300;
            
            // Guardar el libro de trabajo con opciones HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file saved with SVG images.");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


