---
title: "ExportTableOptions.DataTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. Obtiene y establece el DataTable al que se asigna el tipo de datos de las columnas"
type: docs
url: /es/net/aspose.cells/exporttableoptions/datatable/
---
## ExportTableOptions.DataTable property

Obtiene y establece el DataTable al que se asigna el tipo de datos de las columnas.

```csharp
public DataTable DataTable { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyDataTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de muestra a las celdas
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Text1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Text2");

            // Crear DataTable y definir columnas
            DataTable dt = new DataTable();
            dt.Columns.Add("NumericData", typeof(double));
            dt.Columns.Add("TextData", typeof(string));

            // Configurar opciones de exportación
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.Indexes = new int[] { 0, 1 }; // Export both columns
            options.DataTable = dt;

            // Exportar datos a DataTable
            cells.ExportDataTable(0, 0, 3, 2, options);

            // Muestre los datos exportados
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["NumericData"]}, {row["TextData"]}");
            }
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


