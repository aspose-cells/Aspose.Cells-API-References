---
title: "PivotTable.RepeatItemsOnEachPrintedPage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si los encabezados de los elementos de pivote en el área de filas se repiten en cada página impresa para los campos de pivote en forma tabular"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/
---
## PivotTable.RepeatItemsOnEachPrintedPage property

Indica si los títulos del elemento de tabla dinámica en el área de filas se repiten en cada página impresa para los campos de tabla dinámica en forma tabular.

```csharp
public bool RepeatItemsOnEachPrintedPage { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRepeatItemsOnEachPrintedPageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("North");
            worksheet.Cells["A4"].PutValue("South");
            worksheet.Cells["A5"].PutValue("South");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Apples");
            worksheet.Cells["B3"].PutValue("Oranges");
            worksheet.Cells["B4"].PutValue("Apples");
            worksheet.Cells["B5"].PutValue("Oranges");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["C5"].PutValue(2500);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Establecer la configuración de página para imprimir
            worksheet.PageSetup.PrintTitleRows = "$1:$1";
            worksheet.PageSetup.PrintArea = "A1:G20";
            worksheet.PageSetup.FitToPagesTall = 0;
            worksheet.PageSetup.FitToPagesWide = 1;

            // Mostrar el valor actual de RepeatItemsOnEachPrintedPage
            Console.WriteLine("Current RepeatItemsOnEachPrintedPage value: " + pivotTable.RepeatItemsOnEachPrintedPage);

            // Habilitar la repetición de elementos en cada página impresa
            pivotTable.RepeatItemsOnEachPrintedPage = true;
            Console.WriteLine("RepeatItemsOnEachPrintedPage set to: " + pivotTable.RepeatItemsOnEachPrintedPage);

            // Calcular datos para rellenar la tabla dinámica
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableRepeatItemsOnEachPrintedPageDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


