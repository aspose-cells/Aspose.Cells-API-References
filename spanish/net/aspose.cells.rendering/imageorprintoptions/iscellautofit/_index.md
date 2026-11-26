---
title: "ImageOrPrintOptions.IsCellAutoFit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Indica si el ancho y la altura de las celdas se ajustan automáticamente al valor de la celda. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/iscellautofit/
---
## ImageOrPrintOptions.IsCellAutoFit property

Indica si el ancho y la altura de las celdas se ajustan automáticamente al valor de la celda. El valor predeterminado es false.

```csharp
[Obsolete("This property is not used, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCellAutoFit { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, esta propiedad no se usa, por favor elimine esta propiedad. Esta propiedad será eliminada 12 meses después desde agosto de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsCellAutoFitDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer texto de muestra que exceda el ancho de columna predeterminado
            worksheet.Cells["B4"].Value = "This is a long text that demonstrates cell autofit behavior when converting to image.";
            
            // Crear opciones de renderizado de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Demostrar IsCellAutoFit false (predeterminado)
            Console.WriteLine("Default IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithoutAutoFit.png");

            // Cambiar IsCellAutoFit a true
            options.IsCellAutoFit = true;
            Console.WriteLine("Modified IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithAutoFit.png");

            Console.WriteLine("Images created successfully. Compare column widths in output files.");
        }

        private static void SaveAsImage(Worksheet worksheet, ImageOrPrintOptions options, string fileName)
        {
            // Configurar formato de imagen
            options.ImageType = ImageType.Png;

            // Renderizar hoja de cálculo a imagen con opciones especificadas
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, fileName);
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


