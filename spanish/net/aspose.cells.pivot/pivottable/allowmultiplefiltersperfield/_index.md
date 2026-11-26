---
title: "PivotTable.AllowMultipleFiltersPerField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros establecidos en ellos"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/
---
## PivotTable.AllowMultipleFiltersPerField property

Especifica un valor booleano que indica si los campos de una PivotTable pueden tener varios filtros aplicados.

```csharp
public bool AllowMultipleFiltersPerField { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAllowMultipleFiltersPerFieldDemo
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
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Establecer la propiedad AllowMultipleFiltersPerField
            pivotTable.AllowMultipleFiltersPerField = true;
            Console.WriteLine("AllowMultipleFiltersPerField: " + pivotTable.AllowMultipleFiltersPerField);

            // Guarda el libro de trabajo
            workbook.Save("PivotTable_AllowMultipleFiltersPerField.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


