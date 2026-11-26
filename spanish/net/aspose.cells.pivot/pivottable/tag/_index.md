---
title: "PivotTable.Tag"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene y establece una cadena definida por el usuario que está asociada a esta vista de tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/tag/
---
## PivotTable.Tag property

Obtiene y establece una cadena definida por el usuario que está asociada a esta vista de tabla dinámica.

```csharp
public string Tag { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTagDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Establecer y demostrar la propiedad Tag
            pivotTable.Tag = "SamplePivotTableTag";
            Console.WriteLine("Pivot Table Tag: " + pivotTable.Tag);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableTagDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


