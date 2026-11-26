---
title: "ExportTableOptions.ExportAsHtmlString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. Exporta el valor de cadena HTML de las celdas a la DataTable"
type: docs
url: /es/net/aspose.cells/exporttableoptions/exportashtmlstring/
---
## ExportTableOptions.ExportAsHtmlString property

Exporta el valor de cadena HTML de las celdas al DataTable.

```csharp
public bool ExportAsHtmlString { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportAsHtmlStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Establecer el valor de la celda con formato
            cells["A1"].PutValue("abc");
            Style style = cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.Font.Color = System.Drawing.Color.Black;
            cells["A1"].SetStyle(style);

            // Exportar con ExportAsHtmlString
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsHtmlString = true;
            
            DataTable dt = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            
            Console.WriteLine("HTML String: " + dt.Rows[0][0].ToString());
            Console.WriteLine("Expected Format: " + cells["A1"].HtmlString);
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


