---
title: "HtmlSaveOptions.ExportWorksheetCSSSeparately"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exporta el CSS de la hoja de cálculo por separado. El valor predeterminado es false."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportworksheetcssseparately/
---
## HtmlSaveOptions.ExportWorksheetCSSSeparately property

Indica si se exporta el CSS de la hoja de cálculo por separado. El valor predeterminado es false.

```csharp
public bool ExportWorksheetCSSSeparately { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetCSSSeparatelyDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Establecer opciones de guardado HTML con ExportWorksheetCSSSeparately
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportWorksheetCSSSeparately = true;
            
            // Guarda el libro de trabajo como HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with separate CSS saved to: " + outputPath);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


