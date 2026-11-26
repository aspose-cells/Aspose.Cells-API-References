---
title: "ImportTableOptions.DefaultValues"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImportTableOptions. El valor predeterminado para el valor en la tabla es null"
type: docs
url: /es/net/aspose.cells/importtableoptions/defaultvalues/
---
## ImportTableOptions.DefaultValues property

El valor predeterminado para el valor en la tabla es null.

```csharp
public object[] DefaultValues { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyDefaultValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra con valores nulos
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Quantity", typeof(int));
            dataTable.Columns.Add("ExpiryDate", typeof(DateTime));
            
            dataTable.Rows.Add("Bread", 10, DateTime.Now.AddDays(7));
            dataTable.Rows.Add(null, null, null); // Will use default values
            dataTable.Rows.Add("Milk", null, DateTime.Now.AddDays(3));

            ImportTableOptions importOptions = new ImportTableOptions();
            
            // Mostrar estado inicial
            Console.WriteLine("Current DefaultValues: " + (importOptions.DefaultValues == null ? "Not set" : "Set"));

            // Configure valores predeterminados para cada columna
            importOptions.DefaultValues = new object[] { "[Unspecified]", 1, DateTime.Today };

            // Importar datos con manejo de nulos
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Ajustar automáticamente las columnas para una mejor visibilidad
            worksheet.AutoFitColumns();

            workbook.Save("DefaultValuesDemo.xlsx");
            Console.WriteLine("Spreadsheet saved with default values applied to null entries.");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


