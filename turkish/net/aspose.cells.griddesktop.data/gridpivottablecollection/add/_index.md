---
title: "GridPivotTableCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridPivotTableCollection yöntemi. Yeni bir PivotTable önbelleğini bir PivotCaches koleksiyonuna ekler"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridpivottablecollection/add/
---
## Add(string, string, string) {#add_3}

PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable için veri hücre aralığı. Örnek : Sheet1!A1:C8 |
| destCellName | String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | String | Yeni PivotTable raporunun adı. |

### Dönüş Değeri

Yeni eklenen önbellek indeksi.

### Ayrıca Bakınız

* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(Worksheet, GridCellArea, string, string) {#add}

PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.

```csharp
public int Add(Worksheet sourceSheet, GridCellArea sourceArea, string destCellName, 
    string tableName)
```

| Parametre | Açıklama |
| --- | --- |
| sourceSheet | Kaynak çalışma sayfası. |
| sourceArea | Kaynak çalışma sayfasındaki alan. |
| destRow | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satırı. |
| destCol | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütunu. |
| tableName | Yeni PivotTable raporunun adı. |

### Dönüş Değeri

Yeni eklenen önbellek indeksi.

### Ayrıca Bakınız

* class [Worksheet](../../../aspose.cells.griddesktop/worksheet/)
* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, int, int, string) {#add_1}

PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, int destRow, int destCol, 
    string tableName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| worksheetname | String | Kaynak çalışma sayfasının adı. |
| sourceArea | GridCellArea | Kaynak çalışma sayfasındaki alan. |
| destRow | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satırı. |
| destCol | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütunu. |
| tableName | String | Yeni PivotTable raporunun adı. |

### Dönüş Değeri

Yeni eklenen önbellek indeksi.

### Ayrıca Bakınız

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, string, string) {#add_2}

PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, string destCellName, string tableName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| worksheetname | String | Kaynak çalışma sayfasının adı. |
| sourceArea | GridCellArea | Kaynak çalışma sayfasındaki alan. |
| destCellName | String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | String | Yeni PivotTable raporunun adı. |

### Dönüş Değeri

Yeni eklenen önbellek indeksi.

### Ayrıca Bakınız

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


