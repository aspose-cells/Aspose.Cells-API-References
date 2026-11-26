---
title: "ImportTableOptions.InsertRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ImportTableOptions property. Indica si se deben agregar nuevas filas para importar registros de datos"
type: docs
url: /es/net/aspose.cells/importtableoptions/insertrows/
---
## ImportTableOptions.InsertRows property

Indica si se deben agregar filas nuevas al importar registros de datos.

```csharp
public bool InsertRows { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyInsertRowsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear tabla de datos de ejemplo
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            dataTable.Rows.Add(1, "Laptop", 999.99);
            dataTable.Rows.Add(2, "Monitor", 249.99);
            dataTable.Rows.Add(3, "Keyboard", 49.99);

            // Agregar datos existentes a la hoja de cálculo (se desplazarán hacia abajo por la inserción)
            cells["A1"].PutValue("Existing Data");
            cells["A2"].PutValue(100);

            // Establecer opciones de importación con InsertRows = true
            ImportTableOptions options = new ImportTableOptions();
            options.InsertRows = true; // This will insert new rows instead of overwriting
            options.IsFieldNameShown = true;

            // Importar datos comenzando en la fila 1 (insertará filas debajo de los datos existentes)
            cells.ImportData(dataTable, 1, 0, options);

            // Guarda el libro de trabajo
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


