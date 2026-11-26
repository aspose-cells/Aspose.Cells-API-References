---
title: "PivotTable.ItemPrintTitles"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si los nombres de PivotItem deben repetirse en la parte superior de cada página impresa"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/itemprinttitles/
---
## PivotTable.ItemPrintTitles property

Indica si los nombres de PivotItem deben repetirse en la parte superior de cada página impresa.

```csharp
[Obsolete("Use PivotTable.RepeatItemsOnEachPrintedPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ItemPrintTitles { get; set; }
```

### Observaciones

NOTA: Esta propiedad ahora está obsoleta. En su lugar, utilice la propiedad PivotTable.RepeatItemsOnEachPrintedPage. Este método será eliminado 12 meses después a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyItemPrintTitlesDemo
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
            worksheet.Cells["A5"].PutValue("Product D");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(4000);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar el valor actual de ItemPrintTitles
            Console.WriteLine("Current ItemPrintTitles value: " + pivotTable.ItemPrintTitles);

            // Establecer ItemPrintTitles en true (esto está obsoleto, pero se muestra como demostración)
            pivotTable.ItemPrintTitles = true;

            // Alternativamente, use la propiedad no obsoleta
            pivotTable.RepeatItemsOnEachPrintedPage = true;

            // Actualiza y calcula la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableItemPrintTitlesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


