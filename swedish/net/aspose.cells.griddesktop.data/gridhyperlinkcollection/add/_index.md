---
title: "GridHyperlinkCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridHyperlinkCollection metod. Lägger till en hyperlänk i en angiven cell eller ett cellområde"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridhyperlinkcollection/add/
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

Hyperlänkobjektets index.

### Exempel

```csharp
[C#]

Worksheet worksheet = excel.Worksheets[0];
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com");
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls");

[Visual Basic]

Dim worksheet as Worksheet = excel.Worksheets(0)
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com")
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls")

```

### Se även

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Hyperlänkobjektets index.

### Se även

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Hyperlänkobjektets index.

### Se även

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Hyperlänkobjektets index.

### Se även

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, string) {#add_4}

Lägger till en hyperlänk i en angiven cell på rad‑kolumn‑index.

```csharp
public void Add(int row, int col, string url)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex för cellen. |
| kol | Int32 | Kolumnindex för cellen. |
| url | String | URL för hyperlänken. |

### Se även

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


