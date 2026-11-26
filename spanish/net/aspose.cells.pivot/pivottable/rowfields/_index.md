---
title: "PivotTable.RowFields"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Devuelve una PivotFieldCollection que se muestra actualmente como campos de fila"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/rowfields/
---
## PivotTable.RowFields property

Devuelve una [`PivotFieldCollection`](../../pivotfieldcollection/) que se muestra actualmente como campos de fila.

```csharp
public PivotFieldCollection RowFields { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowFieldsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bike";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Bike";
            cells["B3"].Value = "South";
            cells["C3"].Value = 800;
            
            cells["A4"].Value = "Car";
            cells["B4"].Value = "North";
            cells["C4"].Value = 1500;
            
            cells["A5"].Value = "Car";
            cells["B5"].Value = "South";
            cells["C5"].Value = 1200;

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Agregar campos de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Demostrar la propiedad RowFields
            Console.WriteLine("Row Fields Count: " + pivotTable.RowFields.Count);
            Console.WriteLine("First Row Field Name: " + pivotTable.RowFields[0].Name);
            Console.WriteLine("Second Row Field Name: " + pivotTable.RowFields[1].Name);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableRowFieldsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


