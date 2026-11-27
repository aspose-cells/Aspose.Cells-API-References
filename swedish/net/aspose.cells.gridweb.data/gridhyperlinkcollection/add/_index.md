---
title: "GridHyperlinkCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridHyperlinkCollection metod. Lägger till en hyperlänk i en angiven cell eller ett cellområde"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridhyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Lägger till en hyperlänk till en angiven cell eller ett cellområde.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Första raden i hyperlänkområdet. |
| firstColumn | Int32 | Första kolumnen i hyperlänkområdet. |
| totalRows | Int32 | Antal rader i detta hyperlänksområde. |
| totalColumns | Int32 | Antal kolumner i detta hyperlänksområde. |
| adress | String | Adress för hyperlänken. |

### Returvärde

[`GridHyperlink`](../../gridhyperlink/) object index.

### Se även

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, int, int, string) {#add_1}

Lägger till en hyperlänk till en angiven cell eller ett cellområde.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Cellnamn. |
| totalRows | Int32 | Antal rader i detta hyperlänksområde. |
| totalColumns | Int32 | Antal kolumner i detta hyperlänksområde. |
| adress | String | Adress för hyperlänken. |

### Returvärde

[`GridHyperlink`](../../gridhyperlink/) object index.

### Se även

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, string) {#add_2}

Lägger till en hyperlänk i en angiven cell.

```csharp
public int Add(string cellName, string address)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Cellnamn. |
| adress | String | Adress för hyperlänken. |

### Returvärde

[`GridHyperlink`](../../gridhyperlink/) object index.

### Se även

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, string, string, string, string) {#add_3}

Lägger till en hyperlänk till en angiven cell eller ett cellområde.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startCellName | String | Den övre vänstra cellen i området. |
| endCellName | String | Den nedre högra cellen i området. |
| adress | String | Adress för hyperlänken. |
| textToDisplay | String | Texten som ska visas för den angivna hyperlänken. |
| screenTip | String | ScreenTip-texten för den angivna hyperlänken. |

### Returvärde

[`GridHyperlink`](../../gridhyperlink/) object index.

### Se även

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


