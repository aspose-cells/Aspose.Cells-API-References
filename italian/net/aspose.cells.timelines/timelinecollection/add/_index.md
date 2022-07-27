---
title: Add
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati
type: docs
weight: 20
url: /it/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo della sequenza temporale. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo della sequenza temporale. |
| baseFieldName | String | Il nome di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della sequenza temporale

### Esempi

```csharp

[C#]
//Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati
sheet.Timelines.Add(pivot, 10, 5, "date");
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* spazio dei nomi [Aspose.Cells.Timelines](../../timelinecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| destCellName | String | Il nome della cella nell'angolo superiore sinistro dell'intervallo della sequenza temporale. |
| baseFieldName | String | Il nome di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della sequenza temporale

### Esempi

```csharp

[C#]
//Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati
sheet.Timelines.Add(pivot, "i15", "date");
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* spazio dei nomi [Aspose.Cells.Timelines](../../timelinecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo della sequenza temporale. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo della sequenza temporale. |
| baseFieldIndex | Int32 | L'indice di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della sequenza temporale

### Esempi

```csharp

[C#]
//Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati
sheet.Timelines.Add(pivot, 15, 5, 1);
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* spazio dei nomi [Aspose.Cells.Timelines](../../timelinecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| destCellName | String | Il nome della cella nell'angolo superiore sinistro dell'intervallo della sequenza temporale. |
| baseFieldIndex | Int32 | L'indice di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della sequenza temporale

### Esempi

```csharp

[C#]
//Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati
sheet.Timelines.Add(pivot, "i5", 1);
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* spazio dei nomi [Aspose.Cells.Timelines](../../timelinecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo della sequenza temporale. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo della sequenza temporale. |
| baseField | PivotField | Il campo pivot in tabella pivot.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della sequenza temporale

### Esempi

```csharp

[C#]
//Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati
sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* spazio dei nomi [Aspose.Cells.Timelines](../../timelinecollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| destCellName | String | Il nome della cella nell'angolo superiore sinistro dell'intervallo della sequenza temporale. |
| baseField | PivotField | Il campo pivot in tabella pivot.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della sequenza temporale

### Esempi

```csharp

[C#]
//Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati
sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[1]);
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* spazio dei nomi [Aspose.Cells.Timelines](../../timelinecollection)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
