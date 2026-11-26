---
title: "ImportTableOptions.ColumnIndexes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImportTableOptions. Obtiene o establece las columns0based para importar desde la fuente de datos. null significa que se deben importar todas las columnas."
type: docs
url: /es/net/aspose.cells/importtableoptions/columnindexes/
---
## ImportTableOptions.ColumnIndexes property

Obtiene o establece las columnas (basadas en 0) a importar del origen de datos. null significa que se deben importar todas las columnas.

```csharp
public int[] ColumnIndexes { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyColumnIndexesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear DataTable de ejemplo
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Agregar datos de ejemplo
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);
            dataTable.Rows.Add(3, "Product C", 39.99m);

            // Establezca las opciones de importación para importar solo columnas en los índices 0 y 2 (ID y Precio).
            ImportTableOptions options = new ImportTableOptions();
            options.ColumnIndexes = new int[] { 0, 2 };
            options.IsFieldNameShown = true;

            // Importar datos con los índices de columna especificados.
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Guarda el libro de trabajo
            workbook.Save("ColumnIndexesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


