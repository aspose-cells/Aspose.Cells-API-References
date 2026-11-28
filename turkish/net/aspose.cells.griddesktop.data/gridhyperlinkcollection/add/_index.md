---
title: "GridHyperlinkCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridHyperlinkCollection yöntemi. Belirtilen bir hücreye veya hücre aralığına bir hiperbağlantı ekler"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridhyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Köprü aralığının ilk satırı. |
| firstColumn | Int32 | Köprü aralığının ilk sütunu. |
| totalRows | Int32 | Bu köprü aralığındaki satır sayısı. |
| totalColumns | Int32 | Bu köprü aralığındaki sütun sayısı. |
| address | String | Köprünün adresi. |

### Dönüş Değeri

Köprü nesnesi indeksi.

### Örnekler

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

### Ayrıca Bakınız

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, int, int, string) {#add_1}

Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Hücre adı. |
| totalRows | Int32 | Bu köprü aralığındaki satır sayısı. |
| totalColumns | Int32 | Bu köprü aralığındaki sütun sayısı. |
| address | String | Köprünün adresi. |

### Dönüş Değeri

Köprü nesnesi indeksi.

### Ayrıca Bakınız

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, string) {#add_2}

Belirtilen bir hücreye bir hyperlink ekler.

```csharp
public int Add(string cellName, string address)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Hücre adı. |
| address | String | Köprünün adresi. |

### Dönüş Değeri

Köprü nesnesi indeksi.

### Ayrıca Bakınız

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, string, string, string, string) {#add_3}

Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startCellName | String | Aralığın sol üst hücresi. |
| endCellName | String | Aralığın sağ alt hücresi. |
| address | String | Köprünün adresi. |
| textToDisplay | String | Belirtilen köprü için görüntülenecek metin. |
| screenTip | String | Belirtilen bağlantı için screenTip metni. |

### Dönüş Değeri

Köprü nesnesi indeksi.

### Ayrıca Bakınız

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, string) {#add_4}

Satır ve sütun indeksinde belirtilen hücreye bir hyperlink ekler.

```csharp
public void Add(int row, int col, string url)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Hücrenin satır indeksi. |
| col | Int32 | Hücrenin sütun indeksi. |
| url | String | Köprünün URL'si. |

### Ayrıca Bakınız

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


