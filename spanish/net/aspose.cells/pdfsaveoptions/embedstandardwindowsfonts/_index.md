---
title: "PdfSaveOptions.EmbedStandardWindowsFonts"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Verdadero para incrustar fuentes TrueType. Afecta solo a los caracteres ASCII 32127. Las fuentes para códigos de carácter mayores a 127 siempre se incrustan. Las fuentes siempre se incrustan para el estándar PDF/A1a PDF/A1b. El valor predeterminado es true."
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/
---
## PdfSaveOptions.EmbedStandardWindowsFonts property

True para incrustar fuentes TrueType. Afecta solo a los caracteres ASCII 32-127. Las fuentes para códigos de carácter mayores a 127 siempre se incrustan. Las fuentes siempre se incrustan para el estándar PDF/A-1a, PDF/A-1b. El valor predeterminado es true.

```csharp
public bool EmbedStandardWindowsFonts { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedStandardWindowsFontsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF with embedded fonts");

            // Establecer las opciones de guardado PDF con la propiedad EmbedStandardWindowsFonts
            PdfSaveOptions options = new PdfSaveOptions();
            options.EmbedStandardWindowsFonts = true;

            // Guardar en flujo de memoria
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved with embedded fonts: " + (ms.Length > 0));
            }

            // Demostrar la desactivación de la incrustación de fuentes
            options.EmbedStandardWindowsFonts = false;
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved without embedded fonts: " + (ms.Length > 0));
            }
        }
    }
}
```

### Ver también

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


