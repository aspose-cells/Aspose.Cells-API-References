---
title: "Slicer.LockedPosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Indica si el slicer especificado puede ser movido o redimensionado mediante la interfaz de usuario"
type: docs
url: /es/net/aspose.cells.slicers/slicer/lockedposition/
---
## Slicer.LockedPosition property

Indica si el slicer especificado puede moverse o redimensionarse mediante la interfaz de usuario.

```csharp
public bool LockedPosition { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLockedPositionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Crear colección de tablas dinámicas
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Crear una tabla dinámica
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Crear colección de slicers
            SlicerCollection slicers = worksheet.Slicers;
            
            // Agregar un slicer para la tabla dinámica
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];

            // Establecer propiedades del segmentador
            slicer.Caption = "Fruit Slicer";
            slicer.NumberOfColumns = 2;
            slicer.WidthPixel = 200;
            slicer.HeightPixel = 150;

            // Demostrar la propiedad LockedPosition
            slicer.LockedPosition = true; // Lock the slicer position
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Cambiar LockedPosition a false para permitir el movimiento
            slicer.LockedPosition = false;
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Guarda el libro de trabajo
            workbook.Save("SlicerLockedPositionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


