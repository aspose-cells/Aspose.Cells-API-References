---
title: "Cells.ImportDataRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Importa un DataRow al archivo Excel"
type: docs
url: /es/net/aspose.cells/cells/importdatarow/
---
## Cells.ImportDataRow method

Importa un DataRow al archivo Excel.

```csharp
public void ImportDataRow(DataRow dataRow, int row, int firstColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataRow | DataRow | Objeto DataRow. |
| fila | Int32 | Índice de fila. |
| firstColumn | Int32 | Índice de primera columna. |

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataRowWithDataRowInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear un DataTable de ejemplo
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Agregar datos de ejemplo
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Importa la primera fila de DataTable a la hoja de cálculo comenzando en la fila 0, columna 0
            cells.ImportDataRow(dataTable.Rows[0], 0, 0);

            // Guarda el libro de trabajo
            workbook.Save("ImportDataRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


