---
title: "PivotConditionalFormat.ApplyTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotConditionalFormat. Applica il formato condizionale all'intervallo che deve trovarsi nella regione dati"
type: docs
url: /it/net/aspose.cells.pivot/pivotconditionalformat/applyto/
---
## PivotConditionalFormat.ApplyTo method

Applica il formato condizionale all'intervallo che deve trovarsi nella regione dei dati.

```csharp
public void ApplyTo(int row, int column, PivotConditionFormatScopeType scope)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | La riga selezionata. |
| colonna | Int32 | La colonna selezionata. |
| ambito | PivotConditionFormatScopeType | L'ambito |

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
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

            // Aggiungi tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotTableIndex = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotTableIndex];
            
            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Aggiungi formato condizionale
            PivotConditionalFormatCollection pcfCollection = pivotTable.ConditionalFormats;
            PivotConditionalFormat pcf = pcfCollection[pcfCollection.Add()];
            
            // Dimostrare il metodo ApplyTo con parametri specifici
            pcf.ApplyTo(0, 1, PivotConditionFormatScopeType.Field);
            
            // Aggiungi condizione di formato
            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "20";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = System.Drawing.Color.LightGreen;
            
            // Calcola i dati e salva
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatApplyToDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


