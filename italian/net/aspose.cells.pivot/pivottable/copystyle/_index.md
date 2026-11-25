---
title: "PivotTable.CopyStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Copia lo stile nominato da un'altra tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/copystyle/
---
## PivotTable.CopyStyle method

Copia lo stile denominato da un'altra tabella pivot.

```csharp
public void CopyStyle(PivotTable pivotTable)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | PivotTable | Tabella pivot di origine. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCopyStyleWithPivotTableDemo
    {
        public static void Run()
        {
            // Crea cartella di lavoro di origine con tabella pivot
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Sales");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(200);
            
            // Crea tabella pivot di origine (ottieni esplicitamente l'oggetto tabella pivot)
            PivotTable sourcePivotTable = sourceSheet.PivotTables[sourceSheet.PivotTables.Add("PivotTable1", "A1:B3", "C3")];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Applica stile alla tabella pivot di origine
            sourcePivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Crea cartella di lavoro di destinazione con tabella pivot
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Aggiungi la stessa struttura dati
            destSheet.Cells["A1"].PutValue("Product");
            destSheet.Cells["B1"].PutValue("Sales");
            destSheet.Cells["A2"].PutValue("A");
            destSheet.Cells["B2"].PutValue(150);
            destSheet.Cells["A3"].PutValue("B");
            destSheet.Cells["B3"].PutValue(250);
            
            // Crea tabella pivot di destinazione (ottieni esplicitamente l'oggetto tabella pivot)
            PivotTable destPivotTable = destSheet.PivotTables[destSheet.PivotTables.Add("PivotTable2", "A1:B3", "C3")];
            destPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            destPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Copia lo stile dalla tabella pivot di origine a quella di destinazione
            destPivotTable.CopyStyle(sourcePivotTable);
            
            // Salva il risultato
            destWorkbook.Save("PivotTableStyleCopied.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


