---
title: "Cells.ImportDataView"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Importa un DataView en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/importdataview/
---
## Cells.ImportDataView method

Importa un DataView a una hoja de cálculo.

```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataView | DataView | El objeto DataView a importar. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |

### Valor de retorno

Número total de filas importadas

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataViewWithDataViewInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear DataTable de ejemplo
            DataTable table = new DataTable("Products");
            table.Columns.Add("ID", typeof(int));
            table.Columns.Add("Name", typeof(string));
            table.Columns.Add("Price", typeof(decimal));

            // Agregar datos de ejemplo
            table.Rows.Add(1, "Laptop", 999.99m);
            table.Rows.Add(2, "Smartphone", 699.99m);
            table.Rows.Add(3, "Tablet", 399.99m);

            // Crear DataView a partir de DataTable
            DataView dataView = new DataView(table);

            // Importar DataView en la hoja de cálculo comenzando en la fila 0, columna 0
            cells.ImportDataView(dataView, 0, 0);

            // Guarda el libro de trabajo
            workbook.Save("ImportDataViewOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


