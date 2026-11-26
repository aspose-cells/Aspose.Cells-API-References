---
title: "PivotTable.PageFieldOrder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene y establece el orden en que los campos de página se añaden al diseño de los informes de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/pagefieldorder/
---
## PivotTable.PageFieldOrder property

Obtiene y establece el orden en que los campos de página se añaden al diseño del informe de PivotTable.

```csharp
public PrintOrderType PageFieldOrder { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldOrderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Region";
            cells["D1"].Value = "Sales";
            
            // Agregar filas de datos de muestra
            for (int i = 2; i <= 10; i++)
            {
                cells[$"A{i}"].Value = $"Category{(i % 3) + 1}";
                cells[$"B{i}"].Value = $"Product{(i % 4) + 1}";
                cells[$"C{i}"].Value = $"Region{(i % 2) + 1}";
                cells[$"D{i}"].Value = i * 100;
            }

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:D11", "F5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a áreas
            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Category"]);
            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Region"]);
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Product"]);
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);

            // Establecer el orden de los campos de página y el recuento de ajuste
            pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
            pivotTable.PageFieldWrapCount = 2;

            // Guarda el libro de trabajo
            workbook.Save("PivotTablePageFieldOrderDemo_out.xlsx");
        }
    }
}
```

### Ver también

* enum [PrintOrderType](../../../aspose.cells/printordertype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


