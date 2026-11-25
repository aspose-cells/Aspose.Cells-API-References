---
title: "GridValidationCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridValidationCollection. Aggiunge un GridValidation alla collezione. La convalida è applicata alla cella specificata."
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridvalidationcollection/add/
---
## Add(string) {#add_1}

Aggiungi un [`GridValidation`](../../gridvalidation/) alla collezione. La convalida è applicata alla cella specificata.

```csharp
public GridValidation Add(string cellname)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellname | String | Il nome della cella. |

### Valore di ritorno

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Vedi anche

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int) {#add}

Aggiungi un [`GridValidation`](../../gridvalidation/) alla collezione. La convalida è applicata alla cella specificata.

```csharp
public GridValidation Add(int row, int col)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice di riga della cella. |
| col | Int32 | Indice di colonna della cella. |

### Valore di ritorno

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Vedi anche

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, bool, string) {#add_5}

Aggiunge una convalida a una cella specificata per nome della cella.

```csharp
public void Add(string cellName, bool isRequired, string regEx)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Nome della cella della griglia. |
| isRequired | Booleano | Valore che indica se il valore della cella è obbligatorio. |
| regEx | String | Espressione regolare. |

### Vedi anche

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, ICustomValidation) {#add_2}

Aggiunge una convalida a una cella specificata per indice di riga e colonna.

```csharp
public void Add(int row, int col, ICustomValidation customValidation)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice di riga della cella. |
| col | Int32 | Indice di colonna della cella. |
| customValidation | ICustomValidation | Oggetto di convalida personalizzata. |

### Vedi anche

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, bool, string) {#add_3}

Aggiunge una convalida a una cella specificata per indice di riga e colonna.

```csharp
public void Add(int row, int col, bool isRequired, string regEx)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice di riga della cella. |
| col | Int32 | Indice di colonna della cella. |
| isRequired | Booleano | Valore che indica se il valore della cella è obbligatorio. |
| regEx | String | Espressione regolare. |

### Vedi anche

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, ICustomValidation) {#add_4}

Aggiunge una convalida a una cella specificata per nome della cella.

```csharp
public void Add(string cellName, ICustomValidation customValidation)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Nome della cella della griglia. |
| customValidation | ICustomValidation | Oggetto di convalida personalizzata. |

### Vedi anche

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


