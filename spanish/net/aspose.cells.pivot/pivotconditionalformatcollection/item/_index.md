---
title: "PivotConditionalFormatCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotConditionalFormatCollection. Obtiene el objeto pivot FormatCondition en el índice específico"
type: docs
url: /es/net/aspose.cells.pivot/pivotconditionalformatcollection/item/
---
## PivotConditionalFormatCollection indexer

Obtiene el objeto pivot FormatCondition en el índice específico.

```csharp
public PivotConditionalFormat this[int index] { get; }
```

### Valor de retorno

objeto pivot FormatCondition.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar formato condicional
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex]; // Using Item property
            pfc.AddCellArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 10, EndColumn = 10 });

            // Agregar condición de formato
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "90";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // Calcular tabla dinámica y guardar
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### Ver también

* class [PivotConditionalFormat](../../pivotconditionalformat/)
* class [PivotConditionalFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


