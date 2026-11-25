---
title: "PivotField.IsHiddenItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Indica se lo specifico PivotItem è nascosto"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/ishiddenitem/
---
## PivotField.IsHiddenItem method

Indica se lo specifico PivotItem è nascosto.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItem(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice del pivotItem nel pivotField. |

### Valore di ritorno

se il PivotItem specifico è nascosto

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems[int].IsHidden. Questo metodo sarà rimosso 12 mesi dopo, a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e aggiungi dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Country";
            worksheet.Cells["A2"].Value = "USA";
            worksheet.Cells["A3"].Value = "Canada";
            worksheet.Cells["A4"].Value = "UK";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[0];
            
            // Nascondi l'elemento all'indice 1 (Canada)
            rowField.HideItem(1, true);
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Verifica se l'elemento all'indice 1 è nascosto
            bool isHidden = rowField.IsHiddenItem(1);
            Console.WriteLine("Is item at index 1 hidden? " + isHidden);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldIsHiddenItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


