---
title: "Enum PrintingPageType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.PrintingPageType. Indica qué páginas no se imprimirán"
type: docs
url: /es/net/aspose.cells/printingpagetype/
---
## PrintingPageType enumeration

Indica qué páginas no se imprimirán.

```csharp
public enum PrintingPageType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` | Imprime todas las páginas. |
| IgnoreBlank | `1` | No imprimas las páginas cuyas celdas están en blanco. |
| IgnoreStyle | `2` | No imprimas las páginas cuyas celdas solo contienen estilos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintingPageTypeDemo
    {
        public static void PrintingPageTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Llena algunos datos en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("!");

            // Crear PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Establecer PrintingPageType a IgnoreBlank
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;

            // Guardar el libro de trabajo en PDF con las opciones especificadas
            workbook.Save("output_ignore_blank_page.pdf", pdfSaveOptions);

            // Establecer PrintingPageType a IgnoreStyle
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;

            // Guardar el libro de trabajo en PDF con las opciones especificadas
            workbook.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);

            // Establecer PrintingPageType a Default
            pdfSaveOptions.PrintingPageType = PrintingPageType.Default;

            // Guardar el libro de trabajo en PDF con las opciones especificadas
            workbook.Save("output_default_page.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


