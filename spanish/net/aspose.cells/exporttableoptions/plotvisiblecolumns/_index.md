---
title: "ExportTableOptions.PlotVisibleColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. Solo exporta columnas visibles"
type: docs
url: /es/net/aspose.cells/exporttableoptions/plotvisiblecolumns/
---
## ExportTableOptions.PlotVisibleColumns property

Solo exporta columnas visibles.

```csharp
public bool PlotVisibleColumns { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleColumnsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra y ocultar algunas columnas
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            worksheet.Cells["D1"].PutValue("Column4");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data{i-1}_1");
                worksheet.Cells[$"B{i}"].PutValue($"Data{i-1}_2");
                worksheet.Cells[$"C{i}"].PutValue($"Data{i-1}_3");
                worksheet.Cells[$"D{i}"].PutValue($"Data{i-1}_4");
            }
            
            // Ocultar columna C
            worksheet.Cells.HideColumn(2);

            // Exportar datos con PlotVisibleColumns establecido en true
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.PlotVisibleColumns = true;

            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 6, 4, options);
            
            // Genere la salida de los resultados
            Console.WriteLine("Exported DataTable Columns:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.WriteLine(column.ColumnName);
            }
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


