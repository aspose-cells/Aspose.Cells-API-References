---
title: "PivotTable.GrandTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Devuelve la etiqueta que se muestra en el encabezado de la columna o fila del total general. El valor predeterminado es la cadena Grand Total"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/grandtotalname/
---
## PivotTable.GrandTotalName property

Devuelve la etiqueta que se muestra en el encabezado de la columna o fila de total general. El valor predeterminado es la cadena "Grand Total".

```csharp
public string GrandTotalName { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyGrandTotalNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Laptop";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 1500;
            
            worksheet.Cells["A4"].Value = "Phone";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 800;
            
            worksheet.Cells["A5"].Value = "Phone";
            worksheet.Cells["B5"].Value = "South";
            worksheet.Cells["C5"].Value = 1200;

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos de fila y de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar el valor actual de GrandTotalName
            Console.WriteLine("Current GrandTotalName: " + pivotTable.GrandTotalName);

            // Cambiar el GrandTotalName
            pivotTable.GrandTotalName = "Total Summary";

            // Calcular datos y actualizar la tabla dinámica
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


