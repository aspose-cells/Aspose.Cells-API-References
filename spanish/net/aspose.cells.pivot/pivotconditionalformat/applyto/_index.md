---
title: "PivotConditionalFormat.ApplyTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotConditionalFormat. Aplica el formato condicional al rango que debe estar en la región de datos"
type: docs
url: /es/net/aspose.cells.pivot/pivotconditionalformat/applyto/
---
## PivotConditionalFormat.ApplyTo method

Aplica el formato condicional al rango que debe estar en la región de datos.

```csharp
public void ApplyTo(int row, int column, PivotConditionFormatScopeType scope)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | La fila seleccionada. |
| columna | Int32 | La columna seleccionada. |
| alcance | PivotConditionFormatScopeType | El alcance |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodApplyToWithInt32Int32PivotConditionFormatDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Agregar tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotTableIndex = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotTableIndex];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Agregar formato condicional
            PivotConditionalFormatCollection pcfCollection = pivotTable.ConditionalFormats;
            PivotConditionalFormat pcf = pcfCollection[pcfCollection.Add()];
            
            // Demostrar el método ApplyTo con parámetros específicos
            pcf.ApplyTo(0, 1, PivotConditionFormatScopeType.Field);
            
            // Agregar condición de formato
            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "20";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = System.Drawing.Color.LightGreen;
            
            // Calcular datos y guardar
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatApplyToDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


