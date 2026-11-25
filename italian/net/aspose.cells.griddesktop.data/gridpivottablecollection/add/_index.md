---
title: "GridPivotTableCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridPivotTableCollection metodo. Aggiunge una nuova cache PivotTable a una raccolta PivotCaches"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridpivottablecollection/add/
---
## Add(string, string, string) {#add_3}

Aggiunge una nuova cache PivotTable a una raccolta PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle dati per la nuova PivotTable.Esempio : Sheet1!A1:C8 |
| destCellName | String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |

### Valore di ritorno

L'indice della nuova cache aggiunta.

### Vedi anche

* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(Worksheet, GridCellArea, string, string) {#add}

Aggiunge una nuova cache PivotTable a una raccolta PivotCaches.

```csharp
public int Add(Worksheet sourceSheet, GridCellArea sourceArea, string destCellName, 
    string tableName)
```

| Parametro | Descrizione |
| --- | --- |
| sourceSheet | Il foglio di lavoro di origine. |
| sourceArea | L'area nel foglio di lavoro di origine. |
| destRow | La riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| destCol | La colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | Il nome del nuovo report PivotTable. |

### Valore di ritorno

L'indice della nuova cache aggiunta.

### Vedi anche

* class [Worksheet](../../../aspose.cells.griddesktop/worksheet/)
* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, int, int, string) {#add_1}

Aggiunge una nuova cache PivotTable a una raccolta PivotCaches.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, int destRow, int destCol, 
    string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| worksheetname | String | Il nome del foglio di lavoro di origine. |
| sourceArea | GridCellArea | L'area nel foglio di lavoro di origine. |
| destRow | Int32 | La riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| destCol | Int32 | La colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |

### Valore di ritorno

L'indice della nuova cache aggiunta.

### Vedi anche

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, string, string) {#add_2}

Aggiunge una nuova cache PivotTable a una raccolta PivotCaches.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, string destCellName, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| worksheetname | String | Il nome del foglio di lavoro di origine. |
| sourceArea | GridCellArea | L'area nel foglio di lavoro di origine. |
| destCellName | String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |

### Valore di ritorno

L'indice della nuova cache aggiunta.

### Vedi anche

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


