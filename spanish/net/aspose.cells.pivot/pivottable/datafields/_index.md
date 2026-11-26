---
title: "PivotTable.DataFields"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene una PivotFieldCollection que representa todos los campos de datos en una PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/datafields/
---
## PivotTable.DataFields property

Obtiene una [`PivotFieldCollection`](../../pivotfieldcollection/) que representa todos los campos de datos en una PivotTable.

```csharp
public PivotFieldCollection DataFields { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldsDemo
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

            // Agregar una tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Acceder a los campos de datos y demostrar la funcionalidad
            PivotFieldCollection dataFields = pivotTable.DataFields;
            if (dataFields.Count > 0)
            {
                PivotField dataField = dataFields[0];
                Console.WriteLine("Data Field Name: " + dataField.Name);
                Console.WriteLine("Data Field Function: " + dataField.Function);
            }

            // Guarda el libro de trabajo
            workbook.Save("PivotTableDataFieldsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


