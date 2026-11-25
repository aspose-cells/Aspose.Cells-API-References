---
title: "PivotConditionalFormat.AddCellArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotConditionalFormat. Aggiunge un'area basata sulla visualizzazione della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotconditionalformat/addcellarea/
---
## PivotConditionalFormat.AddCellArea method

Aggiunge un'area basata sulla visualizzazione della tabella pivot.

```csharp
public void AddCellArea(CellArea ca)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | L'area della cella. |

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 120;
            cells["B3"].Value = 85;
            cells["B4"].Value = 90;

            // Aggiungi tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Crea un'area di celle per la formattazione condizionale
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 4;
            cellArea.StartColumn = 5;
            cellArea.EndRow = 6;
            cellArea.EndColumn = 7;

            // Aggiungi formato condizionale con area di celle
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.AddCellArea(cellArea);

            // Aggiungi condizione di formato
            int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pcf.FormatConditions[conditionIndex];
            condition.Formula1 = "50";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // Calcola i dati della tabella pivot
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotConditionalFormatWithCellArea.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


