---
title: "PivotConditionalFormat.ScopeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotConditionalFormat. Obtener y establecer el tipo de alcance para el formato condicional de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotconditionalformat/scopetype/
---
## PivotConditionalFormat.ScopeType property

Obtener y establecer el tipo de alcance para el formato condicional de la tabla dinámica.

```csharp
public PivotConditionFormatScopeType ScopeType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatPropertyScopeTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con una tabla dinámica
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(300);

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar formato condicional a la tabla dinámica
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.ScopeType = PivotConditionFormatScopeType.Data;

            // Agregar condición de formato
            FormatConditionCollection fcs = pcf.FormatConditions;
            CellArea area = new CellArea();
            area.StartRow = 4;
            area.EndRow = 6;
            area.StartColumn = 5;
            area.EndColumn = 5;
            int[] conditionIndex = fcs.Add(area, FormatConditionType.CellValue, OperatorType.Between, "100", "200");
            
            // Establecer estilo de formato
            FormatCondition fc = fcs[conditionIndex[0]];
            fc.Style.BackgroundColor = Color.Yellow;

            // Guarda el libro de trabajo
            wb.Save("PivotConditionalFormatScopeTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


