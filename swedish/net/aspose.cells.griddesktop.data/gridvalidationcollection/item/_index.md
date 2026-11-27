---
title: "GridValidationCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridValidationCollection egenskap. Hämtar Hyperlink‑elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridvalidationcollection/item/
---
## GridValidationCollection indexer (1 of 2)

Hämtar Hyperlink-elementet på det angivna indexet.

```csharp
public GridValidation this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Se även

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridValidationCollection indexer (2 of 2)

Hämtar [`GridValidation`](../../gridvalidation/)‑elementet på den angivna cellen. Om ingen validering, returneras null.

```csharp
public GridValidation this[int row, int column] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| row | Raden i cellen. |
| column | Kolumnen i cellen. |

### Returvärde

Elementet på det angivna indexet.

### Anmärkningar

Om det inte finns ett valideringsobjekt på angivet rad‑kolumn‑index, kommer detta att kontrollera kolumnens valideringsobjekt.

### Se även

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


