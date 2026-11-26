---
title: "PivotTable.RowGrand"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si se deben mostrar totales generales para las filas de esta tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/rowgrand/
---
## PivotTable.RowGrand property

Indica si se deben mostrar totales generales para las filas de esta tabla dinámica.

```csharp
[Obsolete("Use PivotTable.ShowRowGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool RowGrand { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use el método PivotTable.ShowRowGrandTotals. Este método será eliminado 12 meses después a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRowGrandDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);
            
            worksheet.Cells["A5"].PutValue("Product A");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(1500);
            
            worksheet.Cells["A6"].PutValue("Product B");
            worksheet.Cells["B6"].PutValue("North");
            worksheet.Cells["C6"].PutValue(2500);

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C6", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar el valor actual de RowGrand
            Console.WriteLine("Current RowGrand value: " + pivotTable.RowGrand);

            // Cambiar la propiedad RowGrand
            pivotTable.RowGrand = false;

            // Calcular datos de tabla dinámica
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTablePropertyRowGrandDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


