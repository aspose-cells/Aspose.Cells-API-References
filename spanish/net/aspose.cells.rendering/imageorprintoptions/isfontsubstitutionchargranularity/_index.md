---
title: "ImageOrPrintOptions.IsFontSubstitutionCharGranularity"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/
---
## ImageOrPrintOptions.IsFontSubstitutionCharGranularity property

Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con él.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Observaciones

El valor predeterminado es false. Primero intentaremos la fuente predeterminada del Libro de trabajo y la de PdfSaveOption/sistema para la fuente de la celda.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configurar la celda con una fuente potencialmente no compatible
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with unavailable font");
            Style style = cell.GetStyle();
            style.Font.Name = "NonExistentFont";
            cell.SetStyle(style);

            // Crear opciones de renderizado de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png, // Namespace reference now valid
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = false
            };

            // Mostrar y modificar el valor de la propiedad
            Console.WriteLine($"Initial IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            
            // Renderizar con la configuración predeterminada
            new SheetRender(worksheet, options).ToImage(0, "BeforeFontSubstitutionChange.png");

            // Cambiar la propiedad y volver a renderizar
            options.IsFontSubstitutionCharGranularity = true;
            Console.WriteLine($"Updated IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            new SheetRender(worksheet, options).ToImage(0, "AfterFontSubstitutionChange.png");

            // Guardar el libro de trabajo como referencia
            workbook.Save("FontSubstitutionDemoWorkbook.xlsx");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


