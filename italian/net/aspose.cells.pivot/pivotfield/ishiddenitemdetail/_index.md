---
title: "PivotField.IsHiddenItemDetail"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Indica se nascondere il dettaglio del PivotItem specifico"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/ishiddenitemdetail/
---
## PivotField.IsHiddenItemDetail method

Indica se nascondere il dettaglio del PivotItem specifico..

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItemDetail(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice del pivotItem nel pivotField. |

### Valore di ritorno

se il dettaglio del PivotItem specifico è nascosto

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems[int].IsDetailHidden. Questo metodo sarà rimosso tra 12 mesi a partire da agosto 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemDetailWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Country";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Japan";
            cells["A3"].Value = "Japan";
            cells["A4"].Value = "USA";
            cells["A5"].Value = "USA";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;
            cells["B5"].Value = 4000;

            // Aggiungi tabella pivot
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Nascondi il dettaglio dell'elemento per l'indice 1 (USA)
            pivotField.HideItemDetail(1, true);
            
            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Verifica se il dettaglio dell'elemento è nascosto
            Console.WriteLine("Is item at index 1 hidden? " + pivotField.IsHiddenItemDetail(1));
            
            // Salva cartella di lavoro
            workbook.Save("PivotFieldIsHiddenItemDetailDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


