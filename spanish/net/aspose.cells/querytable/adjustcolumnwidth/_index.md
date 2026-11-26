---
title: "QueryTable.AdjustColumnWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad QueryTable. Devuelve o establece AdjustColumnWidth del objeto"
type: docs
url: /es/net/aspose.cells/querytable/adjustcolumnwidth/
---
## QueryTable.AdjustColumnWidth property

Devuelve o establece el AdjustColumnWidth del objeto.

```csharp
public bool AdjustColumnWidth { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyAdjustColumnWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo con anchos de columna variables
            worksheet.Cells["A1"].PutValue("Narrow Column");
            worksheet.Cells["B1"].PutValue("Wide Column Data");
            worksheet.Cells["A2"].PutValue("Short");
            worksheet.Cells["B2"].PutValue("This is some very long text that should demonstrate column width adjustment");

            // Establecer manualmente los anchos de columna
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 10); // Initially narrow for wide data

            // Crear una tabla de consulta (simulada ya que la creación real requiere una fuente de datos externa)
            QueryTable queryTable = worksheet.QueryTables[0];

            // Mostrar el valor actual de AdjustColumnWidth
            Console.WriteLine("Initial AdjustColumnWidth value: " + queryTable.AdjustColumnWidth);

            // Establecer AdjustColumnWidth a true y demostrar el efecto
            queryTable.AdjustColumnWidth = true;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);
            Console.WriteLine("After setting to true, columns would auto-adjust to fit content during refresh");

            // Simular la actualización de la tabla de consulta (normalmente ajustaría los anchos de columna)
            // En un escenario real, esto ocurriría cuando la tabla de consulta actualiza sus datos
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=true:");
            Console.WriteLine("Column A width: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width: " + worksheet.Cells.GetColumnWidth(1));

            // Establecer AdjustColumnWidth a false y demostrar el efecto
            queryTable.AdjustColumnWidth = false;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);

            // Simular la actualización nuevamente (ahora preservaría los anchos de columna originales)
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=false:");
            Console.WriteLine("Column A width remains: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width remains: " + worksheet.Cells.GetColumnWidth(1));

            // Guarda el libro de trabajo
            workbook.Save("QueryTableAdjustColumnWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


