---
title: "GridHyperlinkCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridHyperlinkCollection Methode. Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu"
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridhyperlinkcollection/add/
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

Hyperlink-Objektindex.

### Beispiele

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

### Siehe auch

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Hyperlink-Objektindex.

### Siehe auch

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Hyperlink-Objektindex.

### Siehe auch

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Hyperlink-Objektindex.

### Siehe auch

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, string) {#add_4}

Fügt einer angegebenen Zelle bei Zeilen‑Spalten‑Index einen Hyperlink hinzu.

```csharp
public void Add(int row, int col, string url)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex der Zelle. |
| Spalte | Int32 | Spaltenindex der Zelle. |
| URL | String | URL des Hyperlinks. |

### Siehe auch

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


