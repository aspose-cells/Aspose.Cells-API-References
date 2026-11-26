---
title: "PivotTable.DataBodyRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Devuelve un objeto CellArea que representa el rango que contiene el área de datos en la lista entre la fila de encabezado y la fila de inserción. Solo lectura"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/databodyrange/
---
## PivotTable.DataBodyRange property

Devuelve un objeto [`CellArea`](../../../aspose.cells/cellarea/) que representa el rango que contiene el área de datos en la lista entre la fila de encabezado y la fila de inserción. Solo lectura.

```csharp
public CellArea DataBodyRange { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataBodyRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Agregar datos de muestra para la tabla dinámica
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 2500;

            // Agregar tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A7", "A1:B5", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Configurar tabla dinámica
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualizar los datos de la tabla dinámica
            pivot.RefreshData();
            pivot.CalculateData();

            // Demostrar el uso de DataBodyRange
            CellArea dataBodyArea = pivot.DataBodyRange;
            Console.WriteLine($"Data body range: StartRow={dataBodyArea.StartRow}, EndRow={dataBodyArea.EndRow}, StartColumn={dataBodyArea.StartColumn}, EndColumn={dataBodyArea.EndColumn}");

            // Guarda el libro de trabajo
            workbook.Save("PivotTableDataBodyRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


