---
title: "GridHyperlinkCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridHyperlinkCollection Methode. Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridhyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Erste Zeile des Hyperlink-Bereichs. |
| firstColumn | Int32 | Erste Spalte des Hyperlink-Bereichs. |
| totalRows | Int32 | Anzahl der Zeilen in diesem Hyperlink-Bereich. |
| totalColumns | Int32 | Anzahl der Spalten dieses Hyperlink-Bereichs. |
| address | String | Adresse des Hyperlinks. |

### Rückgabewert

[`GridHyperlink`](../../gridhyperlink/) object index.

### Siehe auch

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, int, int, string) {#add_1}

Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Zellname. |
| totalRows | Int32 | Anzahl der Zeilen in diesem Hyperlink-Bereich. |
| totalColumns | Int32 | Anzahl der Spalten dieses Hyperlink-Bereichs. |
| address | String | Adresse des Hyperlinks. |

### Rückgabewert

[`GridHyperlink`](../../gridhyperlink/) object index.

### Siehe auch

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, string) {#add_2}

Fügt einer angegebenen Zelle einen Hyperlink hinzu.

```csharp
public int Add(string cellName, string address)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Zellname. |
| address | String | Adresse des Hyperlinks. |

### Rückgabewert

[`GridHyperlink`](../../gridhyperlink/) object index.

### Siehe auch

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, string, string, string, string) {#add_3}

Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startCellName | String | Die Zelle oben links des Bereichs. |
| endCellName | String | Die Zelle unten rechts des Bereichs. |
| address | String | Adresse des Hyperlinks. |
| textToDisplay | String | Der Text, der für den angegebenen Hyperlink angezeigt werden soll. |
| screenTip | String | Der ScreenTip-Text für den angegebenen Hyperlink. |

### Rückgabewert

[`GridHyperlink`](../../gridhyperlink/) object index.

### Siehe auch

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


