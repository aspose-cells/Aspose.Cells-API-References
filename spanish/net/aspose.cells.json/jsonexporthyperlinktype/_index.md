---
title: "Enum JsonExportHyperlinkType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Json.JsonExportHyperlinkType. Representa el tipo de cómo exportar hipervínculos a json"
type: docs
url: /es/net/aspose.cells.json/jsonexporthyperlinktype/
---
## JsonExportHyperlinkType enumeration

Representa el tipo de cómo exportar hipervínculos a JSON.

```csharp
public enum JsonExportHyperlinkType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DisplayString | `0` | Exportar cadena de visualización |
| Address | `1` | Exportar url |
| HtmlString | `2` | Exportar como cadena html. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonExportHyperlinkTypeDemo
    {
        public static void JsonExportHyperlinkTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo con hipervínculos
            worksheet.Cells["A1"].PutValue("Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.google.com");

            worksheet.Cells["A2"].PutValue("Aspose");
            worksheet.Hyperlinks.Add("A2", 1, 1, "http://www.aspose.com");

            // Crear JsonSaveOptions y establecer ExportHyperlinkType
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.DisplayString;

            // Guardar el libro de trabajo en formato JSON
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksDisplayString.json", saveOptions);

            // Cambiar ExportHyperlinkType a Address y guardar de nuevo
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.Address;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksAddress.json", saveOptions);

            // Cambiar ExportHyperlinkType a HtmlString y guardar de nuevo
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksHtmlString.json", saveOptions);

            Console.WriteLine("Workbooks saved with different hyperlink export types.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Json](../../aspose.cells.json/)
* assembly [Aspose.Cells](../../)


