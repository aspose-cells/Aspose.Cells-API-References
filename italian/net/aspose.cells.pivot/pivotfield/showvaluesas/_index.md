---
title: "PivotField.ShowValuesAs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Mostra i valori del campo dati in un formato di visualizzazione diverso quando è in uso il calcolo ShowDataAs"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## ShowValuesAs(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) {#showvaluesas}

Mostra i valori del campo dati in un formato di visualizzazione diverso quando è in uso il calcolo ShowDataAs.

```csharp
[Obsolete("Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | Il tipo di formato di visualizzazione dei dati. |
| baseField | Int32 | L'indice del campo su cui si basa il calcolo ShowDataAs. |
| baseItemPositionType | PivotItemPositionType | Il tipo di posizione dell'elemento base. |
| baseItem | Int32 | L'indice dell'elemento base su cui si basa il calcolo ShowDataAs. Funziona solo quando baseItemPositionType è personalizzato. |

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodShowValuesAsWithPivotFieldDataDisplayFormatIntDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            worksheet.Name = "PivotData";

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Quarter");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue(1500);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Q1");
            worksheet.Cells["C4"].PutValue(800);
            
            worksheet.Cells["A5"].PutValue("Furniture");
            worksheet.Cells["B5"].PutValue("Q2");
            worksheet.Cells["C5"].PutValue(1200);

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Aggiungi campo riga
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];

            // Aggiungi campo colonna
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];

            // Aggiungi campo dati e configura ShowValuesAs
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.DisplayName = "Sales Diff";
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);

            // Calcola i dati e salva
            pivotTable.CalculateData();
            workbook.Save("PivotTableShowValuesAsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, int, int) {#showvaluesas_1}

Imposta il calcolo \"Show Values As\" per questo campo pivot.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, int baseField, int baseItem)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Tipo del calcolo "Show Values As". |
| baseField | Int32 | Indice del campo base utilizzato per il calcolo. |
| baseItem | Int32 | Indice dell'elemento base per il calcolo. Usa [`PreviousPivotItem`](../../pivotshowvaluessetting/previouspivotitem/) (-1) per l'elemento precedente, [`NextPivotItem`](../../pivotshowvaluessetting/nextpivotitem/) (-2) per l'elemento successivo; i valori non negativi indicano l'indice ordinale di uno specifico elemento pivot. |

### Osservazioni

Solo per campo dati.

### Vedi anche

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, string, string) {#showvaluesas_2}

Configura il calcolo \"Show Values As\" per questo campo dati.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, string baseField, string baseItem)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Il tipo di calcolo per Show Values As. |
| baseField | String | Il nome del campo base utilizzato nel calcolo. |
| baseItem | String | Didascalia di un elemento pivot regolare. Accetta anche parole chiave letterali riservate: `(previous)` per l'elemento precedente, `(next)` per l'elemento successivo. Passa `null` se il tipo di calcolo selezionato non richiede un elemento base. |

### Vedi anche

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


