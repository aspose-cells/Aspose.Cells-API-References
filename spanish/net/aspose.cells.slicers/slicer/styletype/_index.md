---
title: "Slicer.StyleType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Especifique el tipo de estilo incorporado de slicer. El tipo predeterminado es SlicerStyleLight1"
type: docs
url: /es/net/aspose.cells.slicers/slicer/styletype/
---
## Slicer.StyleType property

Especifique el tipo de estilo de segmentador incorporado. El tipo predeterminado es SlicerStyleLight1.

```csharp
public SlicerStyleType StyleType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyStyleTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Agregar slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Establezca propiedades del slicer, incluido StyleType
            slicer.StyleType = SlicerStyleType.SlicerStyleDark2;
            slicer.Caption = "Fruit Selection";
            slicer.NumberOfColumns = 2;
            slicer.Width = 200;
            slicer.Height = 100;

            // Guarda el libro de trabajo
            workbook.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SlicerStyleType](../../slicerstyletype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


