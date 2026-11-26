---
title: "ImportTableOptions.TotalColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImportTableOptions. Obtiene o establece el recuento total de columnas a importar del origen de datos. 1 significa todas las filas del origen de datos dado"
type: docs
url: /es/net/aspose.cells/importtableoptions/totalcolumns/
---
## ImportTableOptions.TotalColumns property

Obtiene o establece el recuento total de columnas a importar del origen de datos. -1 significa todas las filas del origen de datos dado.

```csharp
public int TotalColumns { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalColumnsDemo
    {
        public static void Run()
        {
            // Crear un DataTable de ejemplo
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Agregar datos de ejemplo
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer opciones de importación con TotalColumns = 2 (solo importará las primeras 2 columnas)
            ImportTableOptions importOptions = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalColumns = 2 // Only import first 2 columns (ID and Name)
            };

            // Importar datos comenzando desde la celda A1
            cells.ImportData(dataTable, 0, 0, importOptions);

            // Guarda el libro de trabajo
            workbook.Save("ImportWithTotalColumns.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Data imported with TotalColumns=2. Only first 2 columns were imported.");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


