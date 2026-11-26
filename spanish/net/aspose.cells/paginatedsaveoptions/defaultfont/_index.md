---
title: "PaginatedSaveOptions.DefaultFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Cuando los caracteres en el Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdfimage. Establezca DefaultFont, como MingLiu o MS Gothic, para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells utilizará la fuente predeterminada del sistema para mostrar estos caracteres Unicode."
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/defaultfont/
---
## PaginatedSaveOptions.DefaultFont property

Cuando los caracteres en el Excel son Unicode y no se establece una fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca la propiedad DefaultFont, como MingLiu o MS Gothic, para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode.

```csharp
public string DefaultFont { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("This text will use the default font");
            worksheet.Cells["A2"].PutValue("如果默认字体支持中文，这将显示正确");

            // Configurar opciones de guardado PDF con fuente predeterminada
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultFont = "宋体";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;

            // Guardar como PDF
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


