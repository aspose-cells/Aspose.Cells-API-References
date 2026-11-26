---
title: "ExportTableOptions.Indexes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. Los índices de columnas/filas que deben exportarse"
type: docs
url: /es/net/aspose.cells/exporttableoptions/indexes/
---
## ExportTableOptions.Indexes property

Los índices de columnas/filas que deben exportarse.

```csharp
public int[] Indexes { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyIndexesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("Department");
            worksheet.Cells["D1"].PutValue("Salary");
            worksheet.Cells["E1"].PutValue("Join Date");
            
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["C2"].PutValue("IT");
            worksheet.Cells["D2"].PutValue(5000);
            worksheet.Cells["E2"].PutValue("2020-01-15");
            
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(28);
            worksheet.Cells["C3"].PutValue("HR");
            worksheet.Cells["D3"].PutValue(4500);
            worksheet.Cells["E3"].PutValue("2019-11-20");

            // Crear opciones de exportación y especificar los índices de columnas a exportar (en orden inverso)
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.Indexes = new int[] { 4, 2, 0 }; // Export columns: Join Date, Department, Name

            // Exportar datos con los índices de columna especificados
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 5, options);

            // Mostrar los datos exportados
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
            }
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


