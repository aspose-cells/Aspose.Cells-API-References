---
title: "ImageOrPrintOptions.SaveFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece el tipo de formato de archivo de salida. Soporta Tiff/XPS"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/saveformat/
---
## ImageOrPrintOptions.SaveFormat property

Obtiene o establece el tipo de formato de archivo de salida. Soporta Tiff/XPS

```csharp
[Obsolete("For Tiff/Svg, use ImageType; For Xps, use Workbook.Save(string, SaveOptions) with XpsSaveOptions")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SaveFormat SaveFormat { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, para Tiff/Svg, use [`ImageType`](../imagetype/); para Xps, use [`Save`](../../../aspose.cells/workbook/save/) con [`XpsSaveOptions`](../../../aspose.cells/xpssaveoptions/). Esta propiedad será eliminada 12 meses después, a partir de agosto de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y rellenar con datos de muestra
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells SaveFormat Demonstration");
            
            // Crear una instancia de ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Mostrar el valor inicial de SaveFormat
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Establezca SaveFormat a TIFF y renderice la hoja de cálculo
            options.SaveFormat = SaveFormat.Tiff;
            SheetRender tiffRenderer = new SheetRender(worksheet, options);
            using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
            {
                tiffRenderer.ToTiff(tiffStream);
            }
            Console.WriteLine("Rendered worksheet to TIFF format");

            // Cambie SaveFormat a XPS y renderice nuevamente
            options.SaveFormat = SaveFormat.Xps;
            SheetRender xpsRenderer = new SheetRender(worksheet, options);
            using (FileStream xpsStream = new FileStream("output.xps", FileMode.Create))
            {
                // Nota: SheetRender no admite el formato XPS. En su lugar, se guardará como formato de imagen.
                xpsRenderer.ToImage(0, xpsStream);
            }
            Console.WriteLine("Rendered worksheet to XPS format");
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


