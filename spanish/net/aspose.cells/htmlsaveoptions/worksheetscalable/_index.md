---
title: "HtmlSaveOptions.WorksheetScalable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se hace zoom in o out del html mediante el nivel de zoom de la hoja al guardar el archivo como html; el valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/worksheetscalable/
---
## HtmlSaveOptions.WorksheetScalable property

Indica si se aplica zoom al HTML mediante el nivel de zoom de la hoja de cálculo al guardar el archivo como HTML, el valor predeterminado es false.

```csharp
public bool WorksheetScalable { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWorksheetScalableDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Establecer las opciones de guardado HTML con la propiedad WorksheetScalable
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WorksheetScalable = true;
            
            // Guardar el libro de trabajo con opciones HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, options);
            
            // Verificar que la salida contenga el estilo de escalado
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains scaling: " + htmlContent.Contains("transform: scale"));
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


