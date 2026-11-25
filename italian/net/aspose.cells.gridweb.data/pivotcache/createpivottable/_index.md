---
title: "PivotCache.CreatePivotTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotCache. Crea un report PivotTable in un nuovo foglio"
type: docs
url: /it/net/aspose.cells.gridweb.data/pivotcache/createpivottable/
---
## CreatePivotTable() {#createpivottable}

Crea un report PivotTable in un nuovo foglio.

```csharp
public PivotTable CreatePivotTable()
```

### Valore di ritorno

L'oggetto PivotTable

### Osservazioni

L'esecuzione di questo metodo creerà un oggetto PivotTable e un nuovo foglio di lavoro. Quindi aggiunge l'oggetto PivotTable all'ultima posizione di GridWeb.Worksheets.PivotTables. Se chiami il metodo PivotTable.DataBind(), il report PivotTable verrà disegnato sul foglio di lavoro creato.

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(string) {#createpivottable_3}

Crea un report PivotTable in un nuovo foglio. Il nome dell'oggetto pivotTable

```csharp
public PivotTable CreatePivotTable(string tableName)
```

### Valore di ritorno

L'oggetto PivotTable

### Osservazioni

L'esecuzione di questo metodo creerà un oggetto PivotTable e un nuovo foglio di lavoro. Quindi aggiunge l'oggetto PivotTable all'ultima posizione di GridWeb.Worksheets.PivotTables. Se chiami il metodo PivotTable.DataBind(), il report PivotTable verrà disegnato sul foglio di lavoro creato.

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell) {#createpivottable_1}

Crea un report PivotTable nel foglio di destinazione.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| targetSheet | WebWorksheet | Il foglio su cui verrà disegnato il report pivotTable |
| targetCell | WebCell | La cella di partenza su cui verrà disegnato il report pivotTable |

### Valore di ritorno

L'oggetto PivotTable

### Osservazioni

L'esecuzione di questo metodo creerà un oggetto PivotTable. Quindi aggiunge l'oggetto PivotTable all'ultima posizione di GridWeb.Worksheets.PivotTables. Se chiami il metodo PivotTable.DataBind(), il report PivotTable verrà disegnato sul foglio targetSheet a partire dalla cella targetCell.

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell, string) {#createpivottable_2}

Crea un report PivotTable nel foglio di destinazione.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| targetSheet | WebWorksheet | Il foglio su cui verrà disegnato il report pivotTable |
| targetCell | WebCell | La cella di partenza su cui verrà disegnato il report pivotTable |
| tableName | String | Il nome dell'oggetto pivotTable |

### Valore di ritorno

L'oggetto PivotTable

### Osservazioni

L'esecuzione di questo metodo creerà un oggetto PivotTable con il nome tableName. Quindi aggiunge l'oggetto PivotTable all'ultima posizione di GridWeb.Worksheets.PivotTables. Se chiami il metodo PivotTable.DataBind(), il report PivotTable verrà disegnato sul foglio targetSheet a partire dalla cella targetCell.

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


