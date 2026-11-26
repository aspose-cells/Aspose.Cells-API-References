---
title: "PivotTable.ColumnGrand"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si el informe de PivotTable muestra totales generales para columnas"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/columngrand/
---
## PivotTable.ColumnGrand property

Indica si el informe de PivotTable muestra totales generales para columnas.

```csharp
[Obsolete("Use PivotTable.ShowColumnGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ColumnGrand { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotTable.ShowColumnGrandTotals. Este método será eliminado 12 meses después, a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyColumnGrandDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Mostrar el valor actual de ColumnGrand
            Console.WriteLine("Current ColumnGrand value: " + pivotTable.ColumnGrand);

            // Cambiar la propiedad ColumnGrand
            pivotTable.ColumnGrand = false;

            // Calcular datos para ver el efecto
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableColumnGrandDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


