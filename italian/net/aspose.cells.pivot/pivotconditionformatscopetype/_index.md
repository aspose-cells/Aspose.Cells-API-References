---
title: "Enumerazione PivotConditionFormatScopeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enumerazione Aspose.Cells.Pivot.PivotConditionFormatScopeType. Rappresenta il tipo di ambito della formattazione condizionale della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivotconditionformatscopetype/
---
## PivotConditionFormatScopeType enumeration

Rappresenta il tipo di ambito della formattazione condizionale della PivotTable.

```csharp
public enum PivotConditionFormatScopeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Data | `0` | Indica che la formattazione condizionale è applicata ai campi dati selezionati. |
| Field | `1` | Indica che la formattazione condizionale è applicata alle intersezioni dei campi della PivotTable selezionati. |
| Selection | `2` | Indica che la formattazione condizionale è applicata alle celle selezionate. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotConditionFormatScopeTypeDemo
    {
        public static void PivotConditionFormatScopeTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi alcuni dati al worksheet
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Aggiungi una tabella pivot
            PivotTableCollection pivots = worksheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Aggiungi PivotFormatCondition
            int formatIndex = pivot.PivotFormatConditions.Add();
            PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
            FormatConditionCollection fcc = pfc.FormatConditions;
            fcc.AddArea(pivot.DataBodyRange);
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;

            // Imposta il tipo di ambito per la formattazione condizionale della tabella pivot
            pfc.ScopeType = PivotConditionFormatScopeType.Data;

            pivot.RefreshData();
            pivot.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotConditionFormatScopeTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


