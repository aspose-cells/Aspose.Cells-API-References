---
title: "ExportTableOptions.PlotVisibleCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. Solo exporta celdas visibles"
type: docs
url: /es/net/aspose.cells/exporttableoptions/plotvisiblecells/
---
## ExportTableOptions.PlotVisibleCells property

Solo exporta celdas visibles.

```csharp
public bool PlotVisibleCells { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleCellsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo con algunas filas/columnas ocultas
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");
            
            // Ocultar fila 2 y columna B (índice 1)
            worksheet.Cells.HideRow(1);
            worksheet.Cells.HideColumn(1);

            // Crear opciones de exportación con PlotVisibleCells establecido en true
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                PlotVisibleCells = true,
                PlotVisibleColumns = true,
                PlotVisibleRows = true
            };

            // Exportar solo celdas visibles
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 3, exportOptions);

            // Mostrar los datos exportados (solo se deben exportar celdas visibles)
            Console.WriteLine("Exported Data:");
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


