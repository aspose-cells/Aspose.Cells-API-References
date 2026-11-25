---
title: "PivotField.BaseIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Rappresenta l'indice nei campi pivot di origine"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/baseindex/
---
## PivotField.BaseIndex property

Rappresenta l'indice nei campi pivot di origine.

```csharp
public int BaseIndex { get; set; }
```

### Osservazioni

NOTA: Questo setter di questa proprietà è ora obsoleto. Questo setter sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyBaseIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = "PivotData";
            
            // Dati di esempio
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["B1"].PutValue("Quarter");
            ws.Cells["C1"].PutValue("Sales");
            
            ws.Cells["A2"].PutValue("Electronics");
            ws.Cells["A3"].PutValue("Electronics");
            ws.Cells["A4"].PutValue("Clothing");
            ws.Cells["A5"].PutValue("Clothing");
            
            ws.Cells["B2"].PutValue("Q1");
            ws.Cells["B3"].PutValue("Q2");
            ws.Cells["B4"].PutValue("Q1");
            ws.Cells["B5"].PutValue("Q2");
            
            ws.Cells["C2"].PutValue(1000);
            ws.Cells["C3"].PutValue(1200);
            ws.Cells["C4"].PutValue(800);
            ws.Cells["C5"].PutValue(900);

            // Crea tabella pivot - corretto ottenendo la PivotTable dall'indice
            int pivotIndex = ws.PivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pt = ws.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            int rowIndex = pt.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pt.RowFields[rowIndex];
            
            // Aggiungi campo colonna (verrà usato come campo base)
            int colIndex = pt.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField quarterField = pt.ColumnFields[colIndex];
            
            // Aggiungi campo dati con calcolo normale
            int dataIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pt.DataFields[dataIndex];
            dataField.Function = ConsolidationFunction.Sum;
            
            // Aggiungi secondo campo dati che mostra la differenza dal trimestre precedente
            int diffIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField diffField = pt.DataFields[diffIndex];
            diffField.DisplayName = "QoQ Difference";
            diffField.ShowValuesAs(
                PivotFieldDataDisplayFormat.DifferenceFrom, 
                quarterField.BaseIndex, 
                PivotItemPositionType.Previous,
                0);
            
            // Calcola e salva
            wb.CalculateFormula();
            wb.Save("PivotTableWithBaseIndexDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


