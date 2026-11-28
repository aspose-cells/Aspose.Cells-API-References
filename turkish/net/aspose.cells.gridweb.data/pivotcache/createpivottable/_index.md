---
title: "PivotCache.CreatePivotTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotCache yöntemi. Yeni bir Sayfaya PivotTable raporu oluşturur"
type: docs
url: /tr/net/aspose.cells.gridweb.data/pivotcache/createpivottable/
---
## CreatePivotTable() {#createpivottable}

Yeni bir Sayfaya PivotTable raporu oluşturur.

```csharp
public PivotTable CreatePivotTable()
```

### Dönüş Değeri

PivotTable nesnesi

### Açıklamalar

Bu yöntemi çağırmak bir PivotTable nesnesi ve yeni bir çalışma sayfası oluşturur. Ardından PivotTable nesnesini GridWeb.Worksheets.PivotTables koleksiyonunun son konumuna ekler. PivotTable.DataBind() yöntemini çağırırsanız, PivotTable raporu oluşturulan çalışma sayfasına çizilir.

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(string) {#createpivottable_3}

Yeni bir Sayfaya PivotTable raporu oluşturur. pivotTable nesnesinin adı

```csharp
public PivotTable CreatePivotTable(string tableName)
```

### Dönüş Değeri

PivotTable nesnesi

### Açıklamalar

Bu yöntemi çağırmak bir PivotTable nesnesi ve yeni bir çalışma sayfası oluşturur. Ardından PivotTable nesnesini GridWeb.Worksheets.PivotTables koleksiyonunun son konumuna ekler. PivotTable.DataBind() yöntemini çağırırsanız, PivotTable raporu oluşturulan çalışma sayfasına çizilir.

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell) {#createpivottable_1}

targetSheet'e PivotTable raporu oluşturur.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| targetSheet | WebWorksheet | pivotTable raporunun çizileceği sayfa |
| targetCell | WebCell | pivotTable raporunun çizileceği başlangıç hücresi |

### Dönüş Değeri

PivotTable nesnesi

### Açıklamalar

Bu yöntemi çağırmak bir PivotTable nesnesi oluşturur ve ardından PivotTable nesnesini GridWeb.Worksheets.PivotTables koleksiyonunun son konumuna ekler. PivotTable.DataBind() yöntemini çağırırsanız, PivotTable raporu targetSheet üzerine, targetCell'den başlayarak çizilir.

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell, string) {#createpivottable_2}

targetSheet'e PivotTable raporu oluşturur.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell, string tableName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| targetSheet | WebWorksheet | pivotTable raporunun çizileceği sayfa |
| targetCell | WebCell | pivotTable raporunun çizileceği başlangıç hücresi |
| tableName | String | pivotTable nesnesinin adı |

### Dönüş Değeri

PivotTable nesnesi

### Açıklamalar

Bu yöntemi çağırmak, tableName adını vererek bir PivotTable nesnesi oluşturur ve ardından PivotTable nesnesini GridWeb.Worksheets.PivotTables koleksiyonunun son konumuna ekler. PivotTable.DataBind() yöntemini çağırırsanız, PivotTable raporu targetSheet üzerine, targetCell'den başlayarak çizilir.

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


