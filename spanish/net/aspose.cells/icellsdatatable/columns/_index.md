---
title: "ICellsDataTable.Columns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ICellsDataTable. Obtiene el nombre de las columnas"
type: docs
url: /es/net/aspose.cells/icellsdatatable/columns/
---
## ICellsDataTable.Columns property

Obtiene el nombre de las columnas.

```csharp
public string[] Columns { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyColumnsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["C1"].PutValue("Stock");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["C2"].PutValue(15);

            try
            {
                // Exportar rango de datos a ICellsDataTable
                ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 2, 3);

                // Mostrar los nombres de las columnas
                Console.WriteLine("Column names in the data table:");
                foreach (string column in dataTable.Columns)
                {
                    Console.WriteLine(column);
                }

                // Mostrar el recuento de columnas
                Console.WriteLine($"Total columns: {dataTable.Columns.Length}");

                // Guarda el libro de trabajo
                workbook.Save("ColumnsDemo.xlsx");
                Console.WriteLine("Columns property demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


