---
title: "PivotTable.ShowEmptyRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si se incluyen filas vacías en la tabla"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showemptyrow/
---
## PivotTable.ShowEmptyRow property

Indica si se deben incluir filas vacías en la tabla.

```csharp
public bool ShowEmptyRow { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con algunas filas vacías
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["B2"].Value = "TV";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Electronics";
            worksheet.Cells["B3"].Value = "";
            worksheet.Cells["C3"].Value = "";
            
            worksheet.Cells["A4"].Value = "Furniture";
            worksheet.Cells["B4"].Value = "Chair";
            worksheet.Cells["C4"].Value = 500;
            
            worksheet.Cells["A5"].Value = "Furniture";
            worksheet.Cells["B5"].Value = "";
            worksheet.Cells["C5"].Value = "";

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar el valor actual de ShowEmptyRow
            Console.WriteLine("Initial ShowEmptyRow value: " + pivotTable.ShowEmptyRow);

            // Mostrar filas vacías en la tabla dinámica
            pivotTable.ShowEmptyRow = true;
            Console.WriteLine("ShowEmptyRow set to: " + pivotTable.ShowEmptyRow);

            // Calcular datos para rellenar la tabla dinámica
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowEmptyRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


