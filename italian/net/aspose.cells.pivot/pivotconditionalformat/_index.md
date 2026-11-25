---
title: "Classe PivotConditionalFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotConditionalFormat. Rappresenta il formato condizionale della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotconditionalformat/
---
## PivotConditionalFormat class

Rappresenta il formato condizionale della tabella pivot.

```csharp
public class PivotConditionalFormat
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FormatConditions](../../aspose.cells.pivot/pivotconditionalformat/formatconditions/) { get; } | Ottieni le condizioni per il formato condizionale della tabella pivot. |
| [PivotAreas](../../aspose.cells.pivot/pivotconditionalformat/pivotareas/) { get; } | Ottiene tutte le aree pivot. |
| [RuleType](../../aspose.cells.pivot/pivotconditionalformat/ruletype/) { get; set; } | Ottieni e imposta il tipo di regola per il formato condizionale della tabella pivot. |
| [ScopeType](../../aspose.cells.pivot/pivotconditionalformat/scopetype/) { get; set; } | Ottieni e imposta il tipo di ambito per il formato condizionale della tabella pivot. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddCellArea](../../aspose.cells.pivot/pivotconditionalformat/addcellarea/)(CellArea) | Aggiunge un'area basata sulla visualizzazione della tabella pivot. |
| [AddFieldArea](../../aspose.cells.pivot/pivotconditionalformat/addfieldarea/#addfieldarea)(PivotFieldType, PivotField) | Aggiunge un'area del campo pivot. |
| [AddFieldArea](../../aspose.cells.pivot/pivotconditionalformat/addfieldarea/#addfieldarea_1)(PivotFieldType, string) | Aggiunge un'area del campo pivot. |
| [ApplyTo](../../aspose.cells.pivot/pivotconditionalformat/applyto/)(int, int, PivotConditionFormatScopeType) | Applica il formato condizionale all'intervallo che deve trovarsi nella regione dei dati. |
| [GetCellAreas](../../aspose.cells.pivot/pivotconditionalformat/getcellareas/)() | Ottiene tutte le aree di celle a cui si applica questo formato condizionale. |

### Esempi

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
            
            // Imposta dati di esempio
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
            
            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("=A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            
            // Aggiungi formattazione condizionale
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

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


