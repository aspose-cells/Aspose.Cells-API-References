---
title: "PivotTable.Fields"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Restituisce i campi specifici in base al tipo di campo"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/fields/
---
## PivotTable.Fields method

Ottiene i campi specifici per tipo di campo.

```csharp
[Obsolete("Use PivotField.GetFields(PivotFieldType) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldCollection Fields(PivotFieldType fieldType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | PivotFieldType | il tipo di campo. |

### Valore di ritorno

la collezione dei campi specifici

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.GetFields(PivotFieldType). Questo metodo sarà rimosso tra 12 mesi a partire da maggio 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFieldsWithPivotFieldTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = "Sheet";

            // Dati di esempio
            ws.Cells[0, 0].PutValue("X");
            ws.Cells[0, 1].PutValue("Y");
            ws.Cells[0, 2].PutValue("Data");

            ws.Cells[1, 0].PutValue("A");
            ws.Cells[1, 1].PutValue("C");
            ws.Cells[1, 2].PutValue(10);

            ws.Cells[2, 0].PutValue("A");
            ws.Cells[2, 1].PutValue("D");
            ws.Cells[2, 2].PutValue(25);

            ws.Cells[3, 0].PutValue("B");
            ws.Cells[3, 1].PutValue("C");
            ws.Cells[3, 2].PutValue(30);

            ws.Cells[4, 0].PutValue("B");
            ws.Cells[4, 1].PutValue("D");
            ws.Cells[4, 2].PutValue(45);

            // Crea tabella pivot
            PivotTableCollection ptc = ws.PivotTables;
            int index = ptc.Add("=Sheet!A1:C5", "A7", "PivotTable1");
            PivotTable pt = ptc[index];

            // Aggiungi campi e dimostra il metodo Fields con PivotFieldType
            int fp = pt.AddFieldToArea(PivotFieldType.Row, "X");
            PivotField rowField = pt.Fields(PivotFieldType.Row)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Column, "Y");
            PivotField colField = pt.Fields(PivotFieldType.Column)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
            PivotField dataField = pt.Fields(PivotFieldType.Data)[fp];

            // Aggiungi un secondo campo dati con calcolo percentuale
            fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
            dataField = pt.Fields(PivotFieldType.Data)[fp];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfColumn;

            pt.AddFieldToArea(PivotFieldType.Column, pt.DataField);
            pt.RefreshData();
            pt.CalculateData();

            wb.Save("PivotTableFieldsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


