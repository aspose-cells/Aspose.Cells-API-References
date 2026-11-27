---
title: "GridValidationCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridValidationCollection metod. Lägg till en GridValidation i samlingen. Valideringen tillämpas på den specificerade cellen"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridvalidationcollection/add/
---
## Add(string) {#add_1}

Lägg till en [`GridValidation`](../../gridvalidation/) i samlingen. Valideringen tillämpas på den specificerade cellen.

```csharp
public GridValidation Add(string cellname)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellenamn | String | namnet på cellen. |

### Returvärde

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Se även

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int) {#add}

Lägg till en [`GridValidation`](../../gridvalidation/) i samlingen. Valideringen tillämpas på den specificerade cellen.

```csharp
public GridValidation Add(int row, int col)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex för cellen. |
| kol | Int32 | Kolumnindex för cellen. |

### Returvärde

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Se även

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, bool, string) {#add_5}

Lägger till en validering i en specificerad cell enligt cellnamn.

```csharp
public void Add(string cellName, bool isRequired, string regEx)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Namn på rutcellen. |
| isRequired | Boolean | Värde som indikerar om cellvärdet är obligatoriskt. |
| regEx | String | Reguljärt uttryck. |

### Se även

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, ICustomValidation) {#add_2}

Lägger till en validering i en specificerad cell vid rad‑kolumn‑index.

```csharp
public void Add(int row, int col, ICustomValidation customValidation)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex för cellen. |
| kol | Int32 | Kolumnindex för cellen. |
| customValidation | ICustomValidation | Anpassat valideringsobjekt. |

### Se även

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, bool, string) {#add_3}

Lägger till en validering i en specificerad cell vid rad‑kolumn‑index.

```csharp
public void Add(int row, int col, bool isRequired, string regEx)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex för cellen. |
| kol | Int32 | Kolumnindex för cellen. |
| isRequired | Boolean | Värde som indikerar om cellvärdet är obligatoriskt. |
| regEx | String | Reguljärt uttryck. |

### Se även

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, ICustomValidation) {#add_4}

Lägger till en validering i en specificerad cell enligt cellnamn.

```csharp
public void Add(string cellName, ICustomValidation customValidation)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Namn på rutcellen. |
| customValidation | ICustomValidation | Anpassat valideringsobjekt. |

### Se även

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


