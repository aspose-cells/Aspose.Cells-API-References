---
title: Add
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Aggiungi un nuovo Slicer utilizzando la tabella pivot come origine dati
type: docs
weight: 20
url: /it/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Aggiungi un nuovo Slicer utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| destCellName | String | La cella nell'angolo superiore sinistro dell'intervallo Slicer. |
| baseFieldName | String | Il nome di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice Add Slicer

### Esempi

```csharp

[C#]

slicers.Add(pivot, "E3", "fruit");
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* spazio dei nomi [Aspose.Cells.Slicers](../../slicercollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Aggiungi un nuovo Slicer utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo Slicer. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo Slicer. |
| baseFieldName | String | Il nome di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice Add Slicer

### Esempi

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* spazio dei nomi [Aspose.Cells.Slicers](../../slicercollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Aggiungi un nuovo Slicer utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo Slicer. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo Slicer. |
| baseFieldIndex | Int32 | L'indice di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice Add Slicer

### Esempi

```csharp

[C#]

slicers.Add(pivot, 20, 8, 0);
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* spazio dei nomi [Aspose.Cells.Slicers](../../slicercollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Aggiungi un nuovo Slicer utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| destCellName | String | La cella nell'angolo superiore sinistro dell'intervallo Slicer. |
| baseFieldIndex | Int32 | L'indice di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice Add Slicer

### Esempi

```csharp

[C#]

slicers.Add(pivot, "E20", 0);
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* spazio dei nomi [Aspose.Cells.Slicers](../../slicercollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Aggiungi un nuovo Slicer utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo Slicer. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo Slicer. |
| baseField | PivotField | Il campo pivot in tabella pivot.BaseFields |

### Valore di ritorno

Il nuovo indice Add Slicer

### Esempi

```csharp

[C#]

slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* spazio dei nomi [Aspose.Cells.Slicers](../../slicercollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Aggiungi un nuovo Slicer utilizzando la tabella pivot come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto tabella pivot |
| destCellName | String | La cella nell'angolo superiore sinistro dell'intervallo Slicer. |
| baseField | PivotField | Il campo pivot in tabella pivot.BaseFields |

### Valore di ritorno

Il nuovo indice Add Slicer

### Esempi

```csharp

[C#]

slicers.Add(pivot, "I3", pivot.BaseFields[0]);
```

### Guarda anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* spazio dei nomi [Aspose.Cells.Slicers](../../slicercollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Aggiungi un nuovo Slicer utilizzando ListObjet come origine dati

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | ListObject | Oggetto ListObject |
| index | Int32 | L'indice di ListColumn in ListObject.ListColumns |
| destCellName | String | La cella nell'angolo superiore sinistro dell'intervallo Slicer. |

### Valore di ritorno

Il nuovo indice Add Slicer

### Esempi

```csharp

[C#]

slicers.Add(table, 1, "E38");
```

### Guarda anche

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [SlicerCollection](../../slicercollection)
* spazio dei nomi [Aspose.Cells.Slicers](../../slicercollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Aggiungi un nuovo Slicer utilizzando ListObjet come origine dati

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | ListObject | Oggetto ListObject |
| listColumn | ListColumn | ListColumn in ListObject.ListColumns |
| destCellName | String | La cella nell'angolo superiore sinistro dell'intervallo Slicer. |

### Valore di ritorno

Il nuovo indice Add Slicer

### Esempi

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### Guarda anche

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* spazio dei nomi [Aspose.Cells.Slicers](../../slicercollection)
* assemblea [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Aggiungi un nuovo Slicer utilizzando ListObjet come origine dati

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | ListObject | Oggetto ListObject |
| listColumn | ListColumn | ListColumn in ListObject.ListColumns |
| row | Int32 | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo Slicer. |
| column | Int32 | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo Slicer. |

### Valore di ritorno

Il nuovo indice Add Slicer

### Esempi

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### Guarda anche

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* spazio dei nomi [Aspose.Cells.Slicers](../../slicercollection)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
