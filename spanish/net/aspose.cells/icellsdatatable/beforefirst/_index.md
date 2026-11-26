---
title: "ICellsDataTable.BeforeFirst"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ICellsDataTable. Mueve el cursor al inicio de este objeto justo antes de la primera fila"
type: docs
url: /es/net/aspose.cells/icellsdatatable/beforefirst/
---
## ICellsDataTable.BeforeFirst method

Mueve el cursor al inicio de este objeto, justo antes de la primera fila.

```csharp
public void BeforeFirst()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ICellsDataTableMethodBeforeFirstDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
            DataTable sourceTable = new DataTable("Employees");
            sourceTable.Columns.Add("Name", typeof(string));
            sourceTable.Columns.Add("Department", typeof(string));
            sourceTable.Rows.Add("John Doe", "Engineering");
            sourceTable.Rows.Add("Jane Smith", "Marketing");

            // Importar datos a la hoja de cálculo
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;
            worksheet.Cells.ImportData(sourceTable, 0, 0, importOptions);

            // Obtener ICellsDataTable exportando los datos de la hoja de cálculo
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, sourceTable.Rows.Count + 1, sourceTable.Columns.Count);

            try
            {
                // Restablecer el cursor al inicio de la tabla de datos
                dataTable.BeforeFirst();

                Console.WriteLine("Reading data from ICellsDataTable:");
                while (dataTable.Next())
                {
                    Console.WriteLine(
                        $"Name: {dataTable[0]}, " +
                        $"Department: {dataTable[1]}");
                }

                // Demostrar el restablecimiento del cursor
                dataTable.BeforeFirst();
                Console.WriteLine("\nCursor reset. Reading data again:");
                while (dataTable.Next())
                {
                    Console.WriteLine(
                        $"Name: {dataTable["Name"]}, " +
                        $"Department: {dataTable["Department"]}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing BeforeFirst method: {ex.Message}");
            }

            workbook.Save("ICellsDataTableBeforeFirstDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


