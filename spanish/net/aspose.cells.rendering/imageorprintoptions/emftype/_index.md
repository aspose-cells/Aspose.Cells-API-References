---
title: "ImageOrPrintOptions.EmfType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece un EmfType que especifica el formato del Metafile. El valor predeterminado es EmfPlusDual"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

Obtiene o establece un EmfType que especifica el formato del Metafile. El valor predeterminado es EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmfTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "EMF Type Demo";

            try
            {
                // Crear una instancia de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Establecer el tipo de imagen a EMF
                options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;

                // Crear SheetRender con las opciones
                SheetRender renderer = new SheetRender(worksheet, options);

                // Guardar en formato EMF
                using (MemoryStream stream = new MemoryStream())
                {
                    renderer.ToImage(0, stream);

                    // Mostrar el valor de la propiedad EmfType
                    Console.WriteLine("EmfType value: " + options.EmfRenderSetting);

                    // Guardar el archivo EMF
                    File.WriteAllBytes("output.emf", stream.ToArray());
                    Console.WriteLine("EMF file created successfully.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


