---
title: Add
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Aggiunge una nuova cache di tabella pivot a una raccolta di PivotCaches.
type: docs
weight: 20
url: /it/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string, string) {#add_4}

Aggiunge una nuova cache di tabella pivot a una raccolta di PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | I dati per la nuova cache della tabella pivot. |
| destCellName | String | La cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| tableName | String | Il nome del nuovo report di tabella pivot. |

### Valore di ritorno

Il nuovo indice della cache aggiunto.

### Guarda anche

* class [PivotTableCollection](../../pivottablecollection)
* spazio dei nomi [Aspose.Cells.Pivot](../../pivottablecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_5}

Aggiunge una nuova cache di tabella pivot a una raccolta di PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | I dati per la nuova cache della tabella pivot. |
| destCellName | String | La cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| tableName | String | Il nome del nuovo report di tabella pivot. |
| useSameSource | Boolean | Indica se si utilizza la stessa origine dati quando un'altra tabella pivot esistente ha utilizzato questa origine dati. Se la proprietà è true, verrà risparmiata memoria. |

### Valore di ritorno

Il nuovo indice della cache aggiunto.

### Guarda anche

* class [PivotTableCollection](../../pivottablecollection)
* spazio dei nomi [Aspose.Cells.Pivot](../../pivottablecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_2}

Aggiunge una nuova cache di tabella pivot a una raccolta di PivotCaches.

```csharp
public int Add(string sourceData, int row, int column, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle di dati per la nuova tabella pivot. Esempio: Foglio1!A1:C8 |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| tableName | String | Il nome del nuovo report di tabella pivot. |

### Valore di ritorno

Il nuovo indice della cache aggiunto.

### Guarda anche

* class [PivotTableCollection](../../pivottablecollection)
* spazio dei nomi [Aspose.Cells.Pivot](../../pivottablecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_3}

Aggiunge una nuova cache di tabella pivot a una raccolta di PivotCaches.

```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle di dati per la nuova tabella pivot. Esempio: Foglio1!A1:C8 |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| tableName | String | Il nome del nuovo report di tabella pivot. |
| useSameSource | Boolean | Indica se si utilizza la stessa origine dati quando un'altra tabella pivot esistente ha utilizzato questa origine dati. Se la proprietà è true, verrà risparmiata memoria. |

### Valore di ritorno

Il nuovo indice della cache aggiunto.

### Guarda anche

* class [PivotTableCollection](../../pivottablecollection)
* spazio dei nomi [Aspose.Cells.Pivot](../../pivottablecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_1}

Aggiunge un nuovo oggetto tabella pivot alla raccolta da un'altra tabella pivot.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | PivotTable | La tabella pivot di origine. |
| destCellName | String | La cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| tableName | String | Il nome del nuovo report di tabella pivot. |

### Valore di ritorno

Il nuovo indice di tabella pivot aggiunto.

### Guarda anche

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* spazio dei nomi [Aspose.Cells.Pivot](../../pivottablecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add}

Aggiunge un nuovo oggetto tabella pivot alla raccolta da un'altra tabella pivot.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | PivotTable | La tabella pivot di origine. |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| tableName | String | Il nome del nuovo report di tabella pivot. |

### Valore di ritorno

Il nuovo indice di tabella pivot aggiunto.

### Guarda anche

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* spazio dei nomi [Aspose.Cells.Pivot](../../pivottablecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_7}

Aggiunge un nuovo oggetto tabella pivot alla raccolta con più intervalli di consolidamento come origine dati.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String[] | Gli intervalli di consolidamento multipli, come {"Foglio1!A1:C8","Foglio2!A1:B8"} |
| isAutoPage | Boolean | Indica se creare automaticamente un campo di una singola pagina. Se true, i seguenti parametri pageFields verranno ignorati. |
| pageFields | PivotPageFields | Gli elementi del campo della pagina pivot. |
| destCellName | String | destCellName Il nome del nuovo report di tabella pivot. |
| tableName | String | il nome del nuovo rapporto di tabella pivot. |

### Valore di ritorno

Il nuovo indice di tabella pivot aggiunto.

### Guarda anche

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* spazio dei nomi [Aspose.Cells.Pivot](../../pivottablecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_6}

Aggiunge un nuovo oggetto tabella pivot alla raccolta con più intervalli di consolidamento come origine dati.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String[] | Gli intervalli di consolidamento multipli, come {"Foglio1!A1:C8","Foglio2!A1:B8"} |
| isAutoPage | Boolean | Indica se creare automaticamente un campo di pagina singola. Se true, i seguenti parametri pageFields verranno ignorati |
| pageFields | PivotPageFields | Gli elementi del campo della pagina pivot. |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot. |
| tableName | String | Il nome del nuovo report di tabella pivot. |

### Valore di ritorno

Il nuovo indice di tabella pivot aggiunto.

### Guarda anche

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* spazio dei nomi [Aspose.Cells.Pivot](../../pivottablecollection)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
