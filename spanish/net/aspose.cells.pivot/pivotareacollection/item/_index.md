---
title: "PivotAreaCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotAreaCollection. Obtiene un objeto PivotArea"
type: docs
url: /es/net/aspose.cells.pivot/pivotareacollection/item/
---
## PivotAreaCollection indexer

Obtiene un objeto [`PivotArea`](../../pivotarea/);

```csharp
public PivotArea this[int index] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotAreaCollectionPropertyItemDemo
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
            cells["B2"].Value = 100;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 150;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 200;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A5", "A1:B4", "PivotTable");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar formato condicional
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddCellArea(CellArea.CreateCellArea("A5", "B8"));

            // Acceder a PivotAreas usando la propiedad Item
            PivotArea pivotArea = pfc.PivotAreas[0]; // Using Item indexer
            pivotArea.RuleType = PivotAreaType.All;

            // Agregar condición de formato
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "150";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = Color.Red;

            // Calcular y guardar
            pivot.CalculateData();
            workbook.Save("PivotAreaCollectionPropertyItemDemo_output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


