---
title: "GridHyperlinkCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridHyperlinkCollection yöntemi. Belirtilen bir hücreye veya hücre aralığına bir hiperbağlantı ekler"
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridhyperlinkcollection/add/
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

[`GridHyperlink`](../../gridhyperlink/) object index.

### Ayrıca Bakınız

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

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

[`GridHyperlink`](../../gridhyperlink/) object index.

### Ayrıca Bakınız

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

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

[`GridHyperlink`](../../gridhyperlink/) object index.

### Ayrıca Bakınız

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

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

[`GridHyperlink`](../../gridhyperlink/) object index.

### Ayrıca Bakınız

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


