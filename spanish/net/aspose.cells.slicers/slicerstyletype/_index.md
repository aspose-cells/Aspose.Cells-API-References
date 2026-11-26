---
title: "Enum SlicerStyleType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Slicers.SlicerStyleType enum. Especifique el estilo de la vista del segmentador"
type: docs
url: /es/net/aspose.cells.slicers/slicerstyletype/
---
## SlicerStyleType enumeration

Especifica el estilo de la vista del segmentador

```csharp
public enum SlicerStyleType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | estilo claro incorporado uno |
| SlicerStyleLight2 | `1` | estilo claro incorporado dos |
| SlicerStyleLight3 | `2` | estilo claro incorporado tres |
| SlicerStyleLight4 | `3` | estilo claro incorporado cuatro |
| SlicerStyleLight5 | `4` | estilo claro incorporado cinco |
| SlicerStyleLight6 | `5` | estilo claro incorporado seis |
| SlicerStyleOther1 | `6` | estilo incorporado otro uno |
| SlicerStyleOther2 | `7` | estilo incorporado otro dos |
| SlicerStyleDark1 | `8` | estilo oscuro incorporado uno |
| SlicerStyleDark2 | `9` | estilo oscuro incorporado tow |
| SlicerStyleDark3 | `10` | estilo oscuro incorporado tres |
| SlicerStyleDark4 | `11` | estilo oscuro incorporado cuatro |
| SlicerStyleDark5 | `12` | estilo oscuro incorporado cinco |
| SlicerStyleDark6 | `13` | estilo oscuro incorporado seis |
| Custom | `14` | estilo definido por el usuario, no compatible por ahora |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerStyleTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["B4"].Value = 8;
            sheet.Cells["B5"].Value = 12;

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar slicer
            int slicerIndex = sheet.Slicers.Add(pivot, "G1", pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Establecer estilo del segmentador
            slicer.StyleType = SlicerStyleType.SlicerStyleDark1;
            slicer.NumberOfColumns = 2;

            // Guarda el libro de trabajo
            wb.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


