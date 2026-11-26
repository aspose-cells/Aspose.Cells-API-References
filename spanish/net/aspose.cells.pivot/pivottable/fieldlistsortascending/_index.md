---
title: "PivotTable.FieldListSortAscending"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si los campos en la PivotTable están ordenados en un orden no predeterminado en la lista de campos"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/fieldlistsortascending/
---
## PivotTable.FieldListSortAscending property

Indica si los campos en la PivotTable están ordenados en un orden no predeterminado en la lista de campos.

```csharp
public bool FieldListSortAscending { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyFieldListSortAscendingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["B2"].Value = "Laptop";
            worksheet.Cells["C2"].Value = 1200;
            
            worksheet.Cells["A3"].Value = "Electronics";
            worksheet.Cells["B3"].Value = "Phone";
            worksheet.Cells["C3"].Value = 800;
            
            worksheet.Cells["A4"].Value = "Furniture";
            worksheet.Cells["B4"].Value = "Chair";
            worksheet.Cells["C4"].Value = 150;
            
            worksheet.Cells["A5"].Value = "Furniture";
            worksheet.Cells["B5"].Value = "Table";
            worksheet.Cells["C5"].Value = 250;

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar el valor actual de FieldListSortAscending
            Console.WriteLine("Initial FieldListSortAscending: " + pivotTable.FieldListSortAscending);

            // Mostrar la lista de campos en orden ascendente
            pivotTable.FieldListSortAscending = true;
            Console.WriteLine("FieldListSortAscending set to: " + pivotTable.FieldListSortAscending);

            // Actualiza y calcula la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableFieldListSortAscendingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


