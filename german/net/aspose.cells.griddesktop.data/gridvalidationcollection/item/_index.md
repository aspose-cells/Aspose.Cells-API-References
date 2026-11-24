---
title: "GridValidationCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridValidationCollection-Eigenschaft. Gibt das Hyperlink-Element am angegebenen Index zurück."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridvalidationcollection/item/
---
## GridValidationCollection indexer (1 of 2)

Gibt das Hyperlink-Element am angegebenen Index zurück.

```csharp
public GridValidation this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Siehe auch

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridValidationCollection indexer (2 of 2)

Gibt das [`GridValidation`](../../gridvalidation/)‑Element in der angegebenen Zelle zurück. Wenn keine Validierung vorhanden ist, wird null zurückgegeben.

```csharp
public GridValidation this[int row, int column] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| row | Die Zeile der Zelle. |
| column | Die Spalte der Zelle. |

### Rückgabewert

Das Element am angegebenen Index.

### Hinweise

Wenn kein Validierungsobjekt am angegebenen Zeilen‑Spalten‑Index vorhanden ist, wird das Spalten‑Validierungsobjekt geprüft.

### Siehe auch

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


