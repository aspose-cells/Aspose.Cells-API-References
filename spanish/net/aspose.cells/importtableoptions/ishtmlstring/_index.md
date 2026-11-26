---
title: "ImportTableOptions.IsHtmlString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImportTableOptions. Indica si el valor contiene etiquetas html."
type: docs
url: /es/net/aspose.cells/importtableoptions/ishtmlstring/
---
## ImportTableOptions.IsHtmlString property

Indica si el valor contiene etiquetas HTML.

```csharp
public bool IsHtmlString { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsHtmlStringDemo
    {
        public static void Run()
        {
            // Crear un DataTable con datos de ejemplo que contienen HTML.
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Content");
            table.Columns.Add("Time");
            
            // Agregar una fila con contenido HTML.
            table.Rows.Add("1", "<a href='https://www.example.com'>Example Link</a>", "2:30 PM");

            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Importar el DataTable con IsHtmlString establecido en true.
            worksheet.Cells.ImportData(table, 0, 0, new ImportTableOptions
            {
                IsFieldNameShown = true,
                IsHtmlString = true,
                NumberFormats = new string[] { null, null, "h:mm AM/PM" }
            });

            // Guarda el libro de trabajo
            workbook.Save("HtmlStringImportDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


