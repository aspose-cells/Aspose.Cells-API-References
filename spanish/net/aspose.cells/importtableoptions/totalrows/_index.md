---
title: "ImportTableOptions.TotalRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ImportTableOptions property. Obtiene o establece el recuento total de filas a importar desde la fuente de datos. 1 significa todas las filas de la fuente de datos especificada"
type: docs
url: /es/net/aspose.cells/importtableoptions/totalrows/
---
## ImportTableOptions.TotalRows property

Obtiene o establece el recuento total de filas a importar del origen de datos. -1 significa todas las filas del origen de datos dado.

```csharp
public int TotalRows { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalRowsDemo
    {
        public static void Run()
        {
            // Crear un DataTable de ejemplo
            DataTable table = new DataTable("TestTable");
            table.Columns.Add("Column1", typeof(string));
            table.Columns.Add("Column2", typeof(int));
            
            // Agregar datos de ejemplo
            table.Rows.Add("Item1", 100);
            table.Rows.Add("Item2", 200);
            table.Rows.Add("Item3", 300);

            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear ImportTableOptions con TotalRows establecido en 2 (importará solo las primeras 2 filas)
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalRows = 2 // Only import 2 rows from the DataTable
            };

            // Importar datos con las opciones especificadas
            worksheet.Cells.ImportData(table, 0, 0, options);

            // Guarda el libro de trabajo
            workbook.Save("ImportWithTotalRows.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Data imported with TotalRows=2. Only first 2 rows were imported.");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


