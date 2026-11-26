---
title: "PivotField.DisplayName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Representa el nombre para mostrar del campo dinámico en la vista de tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/displayname/
---
## PivotField.DisplayName property

Representa el nombre de visualización del campo de tabla dinámica en la vista de tabla dinámica.

```csharp
public string DisplayName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Crea un libro y añade datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Establecer nombre para mostrar personalizado para el campo de datos
            pivotTable.DataFields[0].DisplayName = "Total Sales";
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Acceder a la celda usando el nombre para mostrar
            Cell cell = pivotTable.GetCellByDisplayName("Total Sales");
            Console.WriteLine("Cell found at row: {0}, column: {1}", cell.Row, cell.Column);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldDisplayNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


