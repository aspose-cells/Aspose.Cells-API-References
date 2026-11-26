---
title: "PivotTable.ShowPivotStyleRowHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si el encabezado de fila en la tabla dinámica debe tener el estilo aplicado"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showpivotstylerowheader/
---
## PivotTable.ShowPivotStyleRowHeader property

Indica si el encabezado de fila en la tabla dinámica debe tener el estilo aplicado.

```csharp
public bool ShowPivotStyleRowHeader { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleRowHeaderDemo
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

            // Agregar una tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Demostrar la propiedad ShowPivotStyleRowHeader
            pivotTable.ShowPivotStyleRowHeader = true;
            Console.WriteLine("ShowPivotStyleRowHeader is set to: " + pivotTable.ShowPivotStyleRowHeader);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowPivotStyleRowHeaderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


