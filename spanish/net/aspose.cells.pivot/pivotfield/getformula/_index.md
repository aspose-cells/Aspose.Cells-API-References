---
title: "PivotField.GetFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Obtiene la fórmula del campo calculado. Solo funciona para el campo calculado"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

Obtiene la fórmula del campo calculado. Solo funciona para el campo calculado.

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
    public class PivotFieldMethodGetFormulaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;
            
            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo calculado con fórmula
            pivotTable.AddCalculatedField("=ABS('Sales')", "Absolute Sales");
            
            // Obtener la fórmula del campo calculado
            PivotFieldCollection fields = pivotTable.DataFields;
            string formula = fields[fields.Count - 1].GetFormula();
            
            // Mostrar la fórmula
            Console.WriteLine("Calculated field formula: " + formula);
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


