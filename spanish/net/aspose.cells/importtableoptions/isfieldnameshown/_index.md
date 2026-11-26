---
title: "ImportTableOptions.IsFieldNameShown"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImportTableOptions. Indica si el nombre del campo debe importarse"
type: docs
url: /es/net/aspose.cells/importtableoptions/isfieldnameshown/
---
## ImportTableOptions.IsFieldNameShown property

Indica si se debe importar el nombre del campo.

```csharp
public bool IsFieldNameShown { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFieldNameShownDemo
    {
        public static void Run()
        {
            // Crear un DataTable de ejemplo
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Product");
            
            // Agregar datos de ejemplo
            table.Rows.Add(1, "Laptop");
            table.Rows.Add(2, "Smartphone");
            table.Rows.Add(3, "Tablet");

            // Crear un libro de trabajo e importar datos con los nombres de campo mostrados
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;  // Show field names
            options.InsertRows = true;       // Insert new rows
            
            // Importar datos comenzando desde la fila 5, columna 0
            cells.ImportData(table, 5, 0, options);
            
            // Guarda el libro de trabajo
            workbook.Save("ImportDataWithFieldNames.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


