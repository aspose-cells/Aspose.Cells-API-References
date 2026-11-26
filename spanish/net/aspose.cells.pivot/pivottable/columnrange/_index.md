---
title: "PivotTable.ColumnRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Devuelve un objeto CellArea que representa el rango que contiene el área de columna en el informe de PivotTable. Solo lectura"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/columnrange/
---
## PivotTable.ColumnRange property

Devuelve un objeto CellArea que representa el rango que contiene el área de columna en el informe de PivotTable. Solo lectura.

```csharp
public CellArea ColumnRange { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnRangeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;
            
            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Actualizar los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Obtener el rango de columna de la tabla dinámica
            CellArea columnRange = pivotTable.ColumnRange;
            Console.WriteLine("Pivot Table Column Range: " + columnRange);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableColumnRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


