---
title: "PivotTable.ConditionalFormats"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene los formatos condicionales de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/conditionalformats/
---
## PivotTable.ConditionalFormats property

Obtiene los formatos condicionales de la tabla dinámica.

```csharp
public PivotConditionalFormatCollection ConditionalFormats { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyConditionalFormatsDemo
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
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 110;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Agregar campos de fila y de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Agregar formato condicional
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.AddFieldArea(PivotFieldType.Data, pivotTable.DataFields[0]);
            
            // Agregar condición de formato
            int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pcf.FormatConditions[conditionIndex];
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Formula1 = "100";
            condition.Style.BackgroundColor = Color.Red;

            // Guardar el libro de trabajo
            workbook.Save("PivotTableConditionalFormatting.xlsx");
        }
    }
}
```

### Ver también

* class [PivotConditionalFormatCollection](../../pivotconditionalformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


