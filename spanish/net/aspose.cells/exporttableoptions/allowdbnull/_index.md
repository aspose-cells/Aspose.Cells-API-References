---
title: "ExportTableOptions.AllowDBNull"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. Este valor indica si se permiten DBNulls en esta tabla"
type: docs
url: /es/net/aspose.cells/exporttableoptions/allowdbnull/
---
## ExportTableOptions.AllowDBNull property

Este valor indica si se permiten DBNulls en esta tabla.

```csharp
public bool AllowDBNull { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyAllowDBNullDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra con algunas celdas vacías
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue(""); // Empty cell
            worksheet.Cells["B3"].PutValue(25);

            // Exportar con AllowDBNull = true (por defecto)
            ExportTableOptions options1 = new ExportTableOptions
            {
                ExportColumnName = true,
                AllowDBNull = true
            };
            
            DataTable table1 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options1);
            Console.WriteLine("With AllowDBNull=true:");
            Console.WriteLine("Row 2 Name: " + (table1.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table1.Rows[1]["Name"]));

            // Exportar con AllowDBNull = false
            ExportTableOptions options2 = new ExportTableOptions
            {
                ExportColumnName = true,
                AllowDBNull = false
            };
            
            DataTable table2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options2);
            Console.WriteLine("\nWith AllowDBNull=false:");
            Console.WriteLine("Row 2 Name: " + (table2.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table2.Rows[1]["Name"]));
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


