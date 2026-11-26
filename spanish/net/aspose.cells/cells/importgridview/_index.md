---
title: "Cells.ImportGridView"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Importa una grid view a estas celdas"
type: docs
url: /es/net/aspose.cells/cells/importgridview/
---
## Cells.ImportGridView method

Importa una vista de cuadrícula a estas celdas.

```csharp
public int ImportGridView(GridView gridView, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| gridView | GridView | El objeto grid view. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| opciones | ImportTableOptions | opciones de importación. |

### Valor de retorno

El número de fila.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un DataTable para simular los datos de GridView
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Price");
            dataTable.Columns.Add("Stock");

            dataTable.Rows.Add("Product A", 100.5, 50);
            dataTable.Rows.Add("Product B", 200.75, 30);
            dataTable.Rows.Add("Product C", 150.25, 75);

            try
            {
                // Crear ImportTableOptions
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;
                options.InsertRows = true;

                // Importar los datos de DataTable comenzando en la celda B3 (fila 2, columna 1)
                worksheet.Cells.ImportData(dataTable, 2, 1, options);

                Console.WriteLine("Data imported successfully starting at cell B3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


