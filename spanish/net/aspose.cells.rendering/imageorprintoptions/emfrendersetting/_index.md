---
title: "ImageOrPrintOptions.EmfRenderSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Configuración para renderizar metarchivos Emf en el archivo fuente"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/emfrendersetting/
---
## ImageOrPrintOptions.EmfRenderSetting property

Configuración para renderizar metafiles EMF en el archivo fuente.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Observaciones

Los metarchivos EMF identificados como "EMF+ Dual" pueden contener tanto registros EMF+ como registros EMF. Cualquiera de los tipos de registro puede usarse para renderizar la imagen, solo registros EMF+, o solo registros EMF. Cuando EmfPlusPrefer está configurado, los registros EMF+ se analizarán al renderizar la imagen; de lo contrario, solo se analizarán los registros EMF. El valor predeterminado es EmfOnly. Para los frameworks que dependen de .NET System.Drawing.Common, esta configuración se ignora.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con contenido de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "EMF Rendering Setting Test";
            worksheet.Cells["C5"].Value = "Sample Content for Image Rendering";

            // Crear opciones de renderizado de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffCompression = TiffCompression.CompressionLZW;

            // Mostrar la configuración actual
            Console.WriteLine("Default EmfRenderSetting: " + options.EmfRenderSetting);

            // Renderizar con la configuración predeterminada de EMF
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "DefaultEmfSetting.tiff");

            // Cambiar la configuración de renderizado EMF y volver a renderizar
            options.EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer;
            Console.WriteLine("\nModified EmfRenderSetting: " + options.EmfRenderSetting);

            SheetRender modifiedRenderer = new SheetRender(worksheet, options);
            modifiedRenderer.ToImage(0, "ModifiedEmfSetting.tiff");

            Console.WriteLine("\nGenerated TIFF images demonstrating EMF rendering settings.");
        }
    }
}
```

### Ver también

* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


