---
title: "Slicer.NumberOfColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Devuelve o establece el número de columnas en el slicer. El valor predeterminado es 1."
type: docs
url: /es/net/aspose.cells.slicers/slicer/numberofcolumns/
---
## Slicer.NumberOfColumns property

Devuelve o establece el número de columnas en el slicer. El valor predeterminado es 1.

```csharp
public int NumberOfColumns { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Crear datos de muestra para tabla dinámica
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["A2"].Value = "Fruits";
            cells["B2"].Value = "Apple";
            cells["A3"].Value = "Fruits";
            cells["B3"].Value = "Banana";
            cells["A4"].Value = "Vegetables";
            cells["B4"].Value = "Carrot";

            // Crear tabla dinámica - almacenar índice y luego obtener el objeto PivotTable
            int pivotIndex = sheet.PivotTables.Add("D1", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Product");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Agregar slicer conectado a la tabla dinámica
            int slicerIndex = sheet.Slicers.Add(pivotTable, "Category", "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Configurar propiedades del slicer
            slicer.Caption = "Product Categories";
            slicer.TopPixel = 50;
            slicer.LeftPixel = 50;
            slicer.HeightPixel = 150;
            slicer.WidthPixel = 200;

            // Demostrar la propiedad NumberOfColumns
            slicer.NumberOfColumns = 2;

            // Guarda el libro de trabajo
            workbook.Save("SlicerDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


