---
title: "WorkbookDesigner.SortDataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookDesigner. Indica si se ordena la fuente de datos"
type: docs
url: /es/net/aspose.cells/workbookdesigner/sortdatasource/
---
## WorkbookDesigner.SortDataSource property

Indica si se ordena la fuente de datos.

```csharp
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SortDataSource { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. Esta propiedad será eliminada 12 meses después desde octubre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado. La fuente de datos Json se ordenará si el marcador inteligente contiene parámetros ascendente y descendente.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerPropertySortDataSourceDemo
    {
        public static void Run()
        {
            // Crear una DataTable de ejemplo con datos sin ordenar
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID", typeof(int));
            dataTable.Columns.Add("ProductName", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Agregar datos de ejemplo en orden sin ordenar
            dataTable.Rows.Add(3, "Product C", 15.99m);
            dataTable.Rows.Add(1, "Product A", 10.50m);
            dataTable.Rows.Add(2, "Product B", 12.75m);

            // Crear un libro de trabajo con marcadores inteligentes
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configurar marcadores inteligentes en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$Price");

            try
            {
                // Crear instancia de WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Mostrar valor inicial de SortDataSource
                Console.WriteLine($"Initial SortDataSource value: {designer.SortDataSource}");

                // Establecer fuente de datos sin ordenar
                designer.SortDataSource = false;
                designer.SetDataSource(dataTable);
                designer.Process();

                // Guardar el resultado sin ordenar
                workbook.Save("UnsortedOutput.xlsx");
                Console.WriteLine("Unsorted data saved to UnsortedOutput.xlsx");

                // Crear un nuevo libro de trabajo para demostración ordenada
                Workbook sortedWorkbook = new Workbook();
                Worksheet sortedSheet = sortedWorkbook.Worksheets[0];
                sortedSheet.Cells["A1"].PutValue("&=$ProductID");
                sortedSheet.Cells["B1"].PutValue("&=$ProductName");
                sortedSheet.Cells["C1"].PutValue("&=$Price");

                // Crear nuevo diseñador con ordenación habilitada
                WorkbookDesigner sortedDesigner = new WorkbookDesigner(sortedWorkbook);
                sortedDesigner.SortDataSource = true;
                sortedDesigner.SetDataSource(dataTable);
                sortedDesigner.Process();

                // Guardar el resultado ordenado
                sortedWorkbook.Save("SortedOutput.xlsx");
                Console.WriteLine("Sorted data saved to SortedOutput.xlsx");
                Console.WriteLine($"Final SortDataSource value: {sortedDesigner.SortDataSource}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


