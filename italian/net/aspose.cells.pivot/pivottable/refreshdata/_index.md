---
title: "PivotTable.RefreshData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Aggiorna i dati dalla sua fonte dati alla cache pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/refreshdata/
---
## RefreshData() {#refreshdata}

Aggiorna i dati dalla sua fonte dati alla cache pivot.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData()
```

### Osservazioni

Raccoglieremo i dati dalla fonte dati in una cache pivot, quindi calcoleremo i dati nella cache nelle celle. È consigliabile chiamare semplicemente [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) per aggiornare e calcolare tutte le tabelle pivot nel file, invece di aggiornarle una per una. NOTA: questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo [`Refresh`](../../pivotcache/refresh/) e rimuovere il successivo [`CalculateData`](../calculatedata/) perché questa tabella pivot verrà calcolata durante l'aggiornamento di [`PivotCache`](../pivotcache/). Questo metodo sarà rimosso 12 mesi dopo, a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campi di riga e di dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Aggiorna e calcola i dati della tabella pivot
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableRefreshDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RefreshData(PivotTableRefreshOption) {#refreshdata_1}

Aggiorna i dati e le impostazioni della tabella pivot dalla sua fonte dati con opzioni.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzione | PivotTableRefreshOption | Le opzioni per aggiornare la fonte dati della pivot table. |

### Osservazioni

Raccoglieremo i dati dalla fonte dati in una cache pivot, quindi calcoleremo i dati nella cache nelle celle. È consigliabile chiamare semplicemente [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) per aggiornare e calcolare tutte le tabelle pivot nel file, invece di aggiornarle una per una. NOTA: questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo [`Refresh`](../../pivotcache/refresh/) e rimuovere il successivo [`CalculateData`](../calculatedata/) perché questa tabella pivot verrà calcolata durante l'aggiornamento di [`PivotCache`](../pivotcache/). Questo metodo sarà rimosso 12 mesi dopo, a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al foglio di lavoro contenente la tabella pivot
            Worksheet worksheet = workbook.Worksheets["PNL_AFS"];
            
            // Ottieni la prima tabella pivot nel foglio di lavoro
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Configura le opzioni di aggiornamento
            PivotTableRefreshOption refreshOptions = new PivotTableRefreshOption();
            refreshOptions.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Aggiorna i dati della tabella pivot con le opzioni specificate
            pivotTable.RefreshData(refreshOptions);
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro modificata
            workbook.Save("example_modified.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


