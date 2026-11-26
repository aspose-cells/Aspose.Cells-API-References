---
title: "PivotTable.GetCellByDisplayName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Obtiene el objeto Cell por el nombre para mostrar del PivotField"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/getcellbydisplayname/
---
## PivotTable.GetCellByDisplayName method

Obtiene el objeto [`Cell`](../../../aspose.cells/cell/) por el nombre para mostrar del PivotField.

```csharp
public Cell GetCellByDisplayName(string displayName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| displayName | String | el DisplayName del PivotField |

### Valor de retorno

el objeto Cell

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetCellByDisplayNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
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
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Obtener el nombre para mostrar del campo de datos
            string displayName = pivotTable.DataFields[0].DisplayName;

            // Usar el método GetCellByDisplayName
            Cell cell = pivotTable.GetCellByDisplayName(displayName);

            // Mostrar resultados
            Console.WriteLine("Display Name: " + displayName);
            Console.WriteLine("Cell Name: " + (cell != null ? cell.Name : "null"));
            Console.WriteLine("Cell Value: " + (cell != null ? cell.Value.ToString() : "null"));

            // Guarda el libro de trabajo
            workbook.Save("PivotTable_GetCellByDisplayName_Output.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


