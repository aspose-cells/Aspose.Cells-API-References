---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor HtmlSaveOptions. Crea opciones para guardar archivo html"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions() {#constructor}

Crea opciones para guardar un archivo html.

```csharp
public HtmlSaveOptions()
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Inicializar HtmlSaveOptions usando el constructor
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // Guardar como HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file saved to: " + outputPath);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlSaveOptions(SaveFormat) {#constructor_1}

Crea opciones para guardar un archivo htm.

```csharp
public HtmlSaveOptions(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato de archivo. Debe ser uno de los siguientes tipos: Html o MHtml, de lo contrario el formato guardado se establecerá como Html automáticamente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            try
            {
                // Crear HtmlSaveOptions con el parámetro SaveFormat
                HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
                
                // Establecer algunas propiedades
                saveOptions.PageTitle = "Aspose.Cells HTML Export";
                saveOptions.ExportActiveWorksheetOnly = true;
                saveOptions.ExportGridLines = true;
                
                // Guardar el libro de trabajo con HtmlSaveOptions
                workbook.Save("HtmlExportWithOptions.html", saveOptions);
                
                Console.WriteLine("HTML file saved successfully with HtmlSaveOptions(SaveFormat)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HtmlSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


