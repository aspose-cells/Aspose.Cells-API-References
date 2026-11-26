---
title: "Enumeración HtmlExportDataOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.HtmlExportDataOptions. Representa las opciones para exportar datos html"
type: docs
url: /es/net/aspose.cells/htmlexportdataoptions/
---
## HtmlExportDataOptions enumeration

Representa las opciones para exportar datos HTML.

```csharp
public enum HtmlExportDataOptions
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Table | `1` | Exportar archivo a html que solo contiene la parte de tabla. |
| All | `255` | Exportar todos los datos a html. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlExportDataOptionsDemo
    {
        public static void HtmlExportDataOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Doe");
            worksheet.Cells["B3"].PutValue(25);

            // Crear HtmlSaveOptions y establecer HtmlExportDataOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All; // Export all data to HTML

            // Guarde el libro de trabajo en formato HTML
            workbook.Save("HtmlExportDataOptionsExample_All.html", saveOptions);

            // Cambiar HtmlExportDataOptions para exportar solo la parte de tabla
            saveOptions.ExportDataOptions = HtmlExportDataOptions.Table; // Export only the table part

            // Guardar el libro de trabajo en formato HTML nuevamente
            workbook.Save("HtmlExportDataOptionsExample_Table.html", saveOptions);

            Console.WriteLine("HTML files have been saved successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


