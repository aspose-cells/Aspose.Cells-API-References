---
title: "Range.ExportDataTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Exporta los datos de este rango a un objeto DataTable"
type: docs
url: /es/net/aspose.cells/range/exportdatatable/
---
## ExportDataTable() {#exportdatatable}

Exporta los datos de este rango a un objeto DataTable.

```csharp
public DataTable ExportDataTable()
```

### Valor de retorno

Objeto DataTable exportado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(450.75);

            // Crea un rango que contenga los datos
            Aspose.Cells.Range dataRange = worksheet.Cells.CreateRange("A1:B4");

            try
            {
                // Exporta el rango a DataTable
                DataTable dataTable = dataRange.ExportDataTable();

                Console.WriteLine("Data exported successfully to DataTable");
                Console.WriteLine($"DataTable contains {dataTable.Rows.Count} rows and {dataTable.Columns.Count} columns");

                // Mostrar los datos exportados
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}: {row[1]}");
                }

                // Modifica el DataTable e impórtalo de nuevo si es necesario
                dataTable.Rows[0]["Price"] = 1300.00;
                Console.WriteLine("\nModified first product price in DataTable to 1300.00");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error exporting data: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("RangeMethodExportDataTableDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(ExportTableOptions) {#exportdatatable_1}

Exporta los datos de este rango a un objeto DataTable.

```csharp
public DataTable ExportDataTable(ExportTableOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | ExportTableOptions | Las opciones para exportar el rango a DataTable. |

### Valor de retorno

Objeto DataTable exportado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class RangeMethodExportDataTableWithExportTableOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear datos de ejemplo en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Nombra el rango que contiene nuestros datos
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1:B3");
            namedRange.Name = "Names";

            // Exporta el rango nombrado a DataTable con opciones
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            DataTable dataTable = namedRange.ExportDataTable(options);

            // Muestra los resultados
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
            }
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../../exporttableoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


