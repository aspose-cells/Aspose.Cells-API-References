---
title: "HtmlSaveOptions.CellNameAttribute"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Especifica el atributo que indica el CellName a escribir. p. ej., si el valor es id, entonces para la celda A1 la salida será td idA1. El valor predeterminado es nulo"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

Especifica el atributo que indica el CellName a escribir. (p.ej., si el valor es "id", entonces para la celda "A1", la salida será:&lt;td id='A1'&gt;). El valor predeterminado es null.

```csharp
public string CellNameAttribute { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using System.Text.RegularExpressions;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellNameAttributeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con algunos datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["B2"].PutValue(123);

            // Establecer opciones de guardado HTML con CellNameAttribute
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellNameAttribute = "id";
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportActiveWorksheetOnly = true;

            // Guardar a archivo HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            // Verificar que la salida HTML contenga los IDs de celda
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains A1 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='A1'"));
            Console.WriteLine("HTML contains B2 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='B2'"));
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


