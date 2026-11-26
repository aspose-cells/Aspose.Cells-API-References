---
title: "PivotItem.Position"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotItem. Especifica el índice de este elemento en todos los PivotItems del campo"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/position/
---
## PivotItem.Position property

Especifica el índice de este elemento en todos los PivotItems del campo.

```csharp
public int Position { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyPositionDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Orange");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Demuestre la propiedad Position
            PivotField rowField = pivotTable.RowFields[0];
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Before - Name: {item.Name}, Position: {item.Position}");
                item.Position = 0; // Set position to 0
                Console.WriteLine($"After - Name: {item.Name}, Position: {item.Position}");
            }

            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotItemPositionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


