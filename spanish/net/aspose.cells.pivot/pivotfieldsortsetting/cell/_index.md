---
title: "PivotFieldSortSetting.Cell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFieldSortSetting. Ordena por los valores en la fila o columna"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldsortsetting/cell/
---
## PivotFieldSortSetting.Cell property

Ordena por los valores en la fila o columna.

```csharp
public string Cell { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertyCellDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 5;
            cells["B4"].Value = 8;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ordenar por referencia de celda
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A2");
            
            // Demostrar el uso de la propiedad Cell
            Console.WriteLine("Sorting by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Cambiar la celda de ordenación
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A3");
            Console.WriteLine("Changed sort cell to: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Borrar la ordenación de celdas
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
            Console.WriteLine("After clearing cell sort: " + 
                (string.IsNullOrEmpty(pivotTable.RowFields[0].SortSetting.Cell) ? "Empty" : "Has value"));
        }
    }
}
```

### Ver también

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


