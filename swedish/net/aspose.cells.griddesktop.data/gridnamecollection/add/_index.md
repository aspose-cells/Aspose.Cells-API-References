---
title: "GridNameCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridNameCollection‑metod. Definierar ett nytt globalt namn"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridnamecollection/add/
---
## Add(string, string) {#add_1}

Definierar ett nytt globalt namn.

```csharp
public int Add(string text, string refersTo)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Namntekst. Den kan ha bladnamn. |
| refersTo | String | Formeln som namnet är definierat att referera till. Den måste ha ett bladnamn, t.ex. 'sheet hello!'A1:B2. |

### Returvärde

Namnet objektindex.

### Se även

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, string, string) {#add}

Definierar ett nytt namn i det angivna bladet.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| Parameter | Beskrivning |
| --- | --- |
| sheetIndex | Bladindexet där namnet tillämpas. |
| text | Namntekst. Den kan inte ha bladnamn. |
| refersTo | Formeln som namnet är definierat för att referera till. Den måste ha bladnamn, t.ex. 'sheet hello!'A1:B2. |
| sheetIndex | Namnets SheetIndex, indexet börjar från 1. |

### Returvärde

Namnet objektindex.

### Se även

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


