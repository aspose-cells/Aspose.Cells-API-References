---
title: "PivotTable.ShowEmptyCol"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si se deben incluir columnas vacías en la tabla"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showemptycol/
---
## PivotTable.ShowEmptyCol property

Indica si se deben incluir columnas vacías en la tabla

```csharp
public bool ShowEmptyCol { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyColDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar el valor actual de ShowEmptyCol
            Console.WriteLine("Current ShowEmptyCol value: " + pivotTable.ShowEmptyCol);

            // Establecer ShowEmptyCol a false (ocultar columnas vacías)
            pivotTable.ShowEmptyCol = false;
            Console.WriteLine("ShowEmptyCol set to false - empty columns will be hidden");

            // Calcular datos de tabla dinámica
            pivotTable.CalculateData();

            // Guardar el libro con columnas vacías ocultas
            workbook.Save("PivotTableHideEmptyCols.xlsx");

            // Restablecer ShowEmptyCol a true (mostrar columnas vacías)
            pivotTable.ShowEmptyCol = true;
            Console.WriteLine("ShowEmptyCol set to true - empty columns will be shown");

            // Calcular los datos de la tabla dinámica nuevamente
            pivotTable.CalculateData();

            // Guardar el libro con columnas vacías visibles
            workbook.Save("PivotTableShowEmptyCols.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


