---
title: "JsonSaveOptions.ExportHyperlinkType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Representa el tipo de exportación de hipervínculo a JSON"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/exporthyperlinktype/
---
## JsonSaveOptions.ExportHyperlinkType property

Representa el tipo de exportación de hipervínculo a json.

```csharp
public JsonExportHyperlinkType ExportHyperlinkType { get; set; }
```

### Observaciones

El valor predeterminado es DisplayString;

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Json;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportHyperlinkTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue un hipervínculo a la celda A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Establecer opciones de exportación para JSON
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            
            // Guardar el libro de trabajo a JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            // Verificar que la salida contenga el hipervínculo
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine("JSON content contains hyperlink: " + 
                jsonContent.Contains("https://www.aspose.com"));
        }
    }
}
```

### Ver también

* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


