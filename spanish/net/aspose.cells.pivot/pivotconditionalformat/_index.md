---
title: "Clase PivotConditionalFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotConditionalFormat. Representa el formato condicional de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotconditionalformat/
---
## PivotConditionalFormat class

Representa el formato condicional de la tabla dinámica.

```csharp
public class PivotConditionalFormat
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FormatConditions](../../aspose.cells.pivot/pivotconditionalformat/formatconditions/) { get; } | Obtener condiciones para el formato condicional de la tabla dinámica. |
| [PivotAreas](../../aspose.cells.pivot/pivotconditionalformat/pivotareas/) { get; } | Obtiene todas las áreas de la tabla dinámica. |
| [RuleType](../../aspose.cells.pivot/pivotconditionalformat/ruletype/) { get; set; } | Obtener y establecer el tipo de regla para el formato condicional de la tabla dinámica. |
| [ScopeType](../../aspose.cells.pivot/pivotconditionalformat/scopetype/) { get; set; } | Obtener y establecer el tipo de alcance para el formato condicional de la tabla dinámica. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddCellArea](../../aspose.cells.pivot/pivotconditionalformat/addcellarea/)(CellArea) | Agrega un área basada en la vista de la tabla dinámica. |
| [AddFieldArea](../../aspose.cells.pivot/pivotconditionalformat/addfieldarea/#addfieldarea)(PivotFieldType, PivotField) | Agrega un área del campo de tabla dinámica. |
| [AddFieldArea](../../aspose.cells.pivot/pivotconditionalformat/addfieldarea/#addfieldarea_1)(PivotFieldType, string) | Agrega un área del campo de tabla dinámica. |
| [ApplyTo](../../aspose.cells.pivot/pivotconditionalformat/applyto/)(int, int, PivotConditionFormatScopeType) | Aplica el formato condicional al rango que debe estar en la región de datos. |
| [GetCellAreas](../../aspose.cells.pivot/pivotconditionalformat/getcellareas/)() | Obtiene todas las áreas de celdas donde se aplica este formato condicional. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotClassPivotConditionalFormatDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Establecer datos de muestra
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";
            
            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;
            
            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;
            
            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("=A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            
            // Agregar formato condicional
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddFieldArea(PivotFieldType.Data, pivot.DataFields[0]);
            
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[conditionIndex];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;
            
            pivot.RefreshData();
            book.Save("PivotConditionalFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


