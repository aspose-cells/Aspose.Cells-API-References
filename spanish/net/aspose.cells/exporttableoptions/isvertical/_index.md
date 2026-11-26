---
title: "ExportTableOptions.IsVertical"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. True si una fila en el archivo Workbook representa una fila en el DataTable. False si una columna en el archivo Workbook representa una fila en el DataTable"
type: docs
url: /es/net/aspose.cells/exporttableoptions/isvertical/
---
## ExportTableOptions.IsVertical property

True si una fila en el archivo Workbook representa una fila en el DataTable. False si una columna en el archivo Workbook representa una fila en el DataTable.

```csharp
public bool IsVertical { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyIsVerticalDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear datos de muestra en la hoja de cálculo
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(25);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(30);

            // Crear DataTable
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));

            // Establecer ExportTableOptions con IsVertical = true
            ExportTableOptions options = new ExportTableOptions();
            options.IsVertical = true;
            options.ExportColumnName = true;
            options.DataTable = dt;

            // Exportar datos verticalmente
            cells.ExportDataTable(0, 0, 2, 2, options);

            // Mostrar la DataTable exportada
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}");
            }
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


