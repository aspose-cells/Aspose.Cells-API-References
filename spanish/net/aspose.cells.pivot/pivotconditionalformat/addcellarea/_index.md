---
title: "PivotConditionalFormat.AddCellArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotConditionalFormat. Añade un área basada en la vista de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotconditionalformat/addcellarea/
---
## PivotConditionalFormat.AddCellArea method

Agrega un área basada en la vista de la tabla dinámica.

```csharp
public void AddCellArea(CellArea ca)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | El área de celda. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodAddCellAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 120;
            cells["B3"].Value = 85;
            cells["B4"].Value = 90;

            // Agregar tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Crear un área de celdas para formato condicional
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 4;
            cellArea.StartColumn = 5;
            cellArea.EndRow = 6;
            cellArea.EndColumn = 7;

            // Agregar formato condicional con área de celdas
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.AddCellArea(cellArea);

            // Agregar condición de formato
            int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pcf.FormatConditions[conditionIndex];
            condition.Formula1 = "50";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // Calcular datos de tabla dinámica
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotConditionalFormatWithCellArea.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


