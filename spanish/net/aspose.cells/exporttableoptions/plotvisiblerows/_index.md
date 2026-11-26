---
title: "ExportTableOptions.PlotVisibleRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. Solo exporta filas visibles"
type: docs
url: /es/net/aspose.cells/exporttableoptions/plotvisiblerows/
---
## ExportTableOptions.PlotVisibleRows property

Solo exporta filas visibles.

```csharp
public bool PlotVisibleRows { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleRowsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear datos de ejemplo en la hoja de cálculo
            cells["A1"].PutValue("Column1");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);
            cells["A4"].PutValue(30);

            // Ocultar fila 3 (índice 2) que contiene el valor 20
            worksheet.Cells.HideRow(2);

            // Crear un DataTable para exportar
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Column1", typeof(int));

            // Configurar opciones de exportación
            ExportTableOptions options = new ExportTableOptions();
            options.PlotVisibleRows = true; // Only export visible rows
            options.ExportColumnName = true;
            options.DataTable = dataTable;

            // Exportar datos (debería omitir la fila oculta)
            cells.ExportDataTable(0, 0, 4, 1, options);

            // Mostrar los datos exportados
            Console.WriteLine("Exported Data (PlotVisibleRows=true):");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine(row["Column1"]);
            }
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


