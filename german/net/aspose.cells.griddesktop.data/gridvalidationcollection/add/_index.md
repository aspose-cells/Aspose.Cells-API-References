---
title: "GridValidationCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridValidationCollection-Methode. Fügt eine GridValidation zur Sammlung hinzu. Die Validierung wird auf die angegebene Zelle angewendet"
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridvalidationcollection/add/
---
## Add(string) {#add_1}

Füge eine [`GridValidation`](../../gridvalidation/) zur Sammlung hinzu. Die Validierung wird auf die angegebene Zelle angewendet.

```csharp
public GridValidation Add(string cellname)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellname | String | Der Name der Zelle. |

### Rückgabewert

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Siehe auch

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int) {#add}

Füge eine [`GridValidation`](../../gridvalidation/) zur Sammlung hinzu. Die Validierung wird auf die angegebene Zelle angewendet.

```csharp
public GridValidation Add(int row, int col)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex der Zelle. |
| Spalte | Int32 | Spaltenindex der Zelle. |

### Rückgabewert

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Siehe auch

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, bool, string) {#add_5}

Fügt einer angegebenen Zelle per Zellnamen eine Validierung hinzu.

```csharp
public void Add(string cellName, bool isRequired, string regEx)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Name der Rasterzelle. |
| isRequired | Boolean | Wert, der angibt, ob ein Zellenwert erforderlich ist. |
| regEx | String | Regulärer Ausdruck. |

### Siehe auch

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, ICustomValidation) {#add_2}

Fügt einer angegebenen Zelle am Zeilen‑ und Spaltenindex eine Validierung hinzu.

```csharp
public void Add(int row, int col, ICustomValidation customValidation)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex der Zelle. |
| Spalte | Int32 | Spaltenindex der Zelle. |
| customValidation | ICustomValidation | Benutzerdefiniertes Validierungsobjekt. |

### Siehe auch

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, bool, string) {#add_3}

Fügt einer angegebenen Zelle am Zeilen‑ und Spaltenindex eine Validierung hinzu.

```csharp
public void Add(int row, int col, bool isRequired, string regEx)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex der Zelle. |
| Spalte | Int32 | Spaltenindex der Zelle. |
| isRequired | Boolean | Wert, der angibt, ob ein Zellenwert erforderlich ist. |
| regEx | String | Regulärer Ausdruck. |

### Siehe auch

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, ICustomValidation) {#add_4}

Fügt einer angegebenen Zelle per Zellnamen eine Validierung hinzu.

```csharp
public void Add(string cellName, ICustomValidation customValidation)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Name der Rasterzelle. |
| customValidation | ICustomValidation | Benutzerdefiniertes Validierungsobjekt. |

### Siehe auch

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


