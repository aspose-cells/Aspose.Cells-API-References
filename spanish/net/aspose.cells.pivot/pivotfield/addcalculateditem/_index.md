---
title: "PivotField.AddCalculatedItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Añade un elemento de fórmula calculada al campo pivote."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/addcalculateditem/
---
## PivotField.AddCalculatedItem method

Agrega un elemento de fórmula calculada al pivot field.

```csharp
public void AddCalculatedItem(string name, string formula)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre del elemento. |
| fórmula | String | La fórmula del elemento pivote. |

### Observaciones

Solo admite añadir elementos calculados al campo de fila/columna.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodAddCalculatedItemWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "grape";
            sheet.Cells["A3"].Value = "kiwi";
            sheet.Cells["A4"].Value = "grape";
            sheet.Cells["A5"].Value = "kiwi";
            
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 50;
            sheet.Cells["B3"].Value = 70;
            sheet.Cells["B4"].Value = 30;
            sheet.Cells["B5"].Value = 20;

            // Crea una tabla dinámica con los parámetros correctos
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtenga el campo pivote y añada el elemento calculado.
            PivotField fruitField = pivotTable.RowFields[0];
            fruitField.AddCalculatedItem("grape_kiwi_total", "=grape + kiwi");
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldAddCalculatedItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


