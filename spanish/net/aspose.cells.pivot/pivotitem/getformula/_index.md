---
title: "PivotItem.GetFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotItem. Obtiene la fórmula de este elemento calculado. Solo funciona cuando este elemento es un elemento calculado"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/getformula/
---
## PivotItem.GetFormula method

Obtiene la fórmula de este elemento calculado. Solo funciona cuando este elemento es calculado.

```csharp
public string GetFormula()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetFormulaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
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

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Obtenga la fórmula de los elementos pivot
            string rowItemFormula = pivotTable.RowFields[0].PivotItems[0].GetFormula();
            string dataFieldFormula = pivotTable.DataFields[0].GetFormula();

            Console.WriteLine("Row Item Formula: " + rowItemFormula);
            Console.WriteLine("Data Field Formula: " + dataFieldFormula);
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


