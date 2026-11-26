---
title: "HtmlSaveOptions.ExportSingleTab"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exporta la única pestaña cuando el archivo solo tiene una hoja de cálculo. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportsingletab/
---
## HtmlSaveOptions.ExportSingleTab property

Indica si se exporta la pestaña única cuando el archivo tiene solo una hoja de cálculo. El valor predeterminado es false.

```csharp
public bool ExportSingleTab { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportSingleTabDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear opciones de guardado HTML con ExportSingleTab establecido en true
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportSingleTab = true,
                ExportImagesAsBase64 = true
            };

            // Guarda el libro de trabajo como HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "SingleTabExport.html");
            workbook.Save(outputPath, options);

            Console.WriteLine("HTML file with single tab export created successfully: " + outputPath);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


