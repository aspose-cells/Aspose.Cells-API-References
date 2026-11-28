---
title: "GridWorksheet.CreateSubtotal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridWorksheet yöntemi. Sayfada ara toplam oluşturur."
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridworksheet/createsubtotal/
---
## CreateSubtotal(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) {#createsubtotal_1}

Sayfada ara toplam oluşturur.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnNameRowIndex | Int32 | Sütun adı satırının satır indeksi. |
| dataRows | Int32 | Veri satırlarının sayısı. |
| groupByColumnIndex | Int32 | Gruplanacak sütunun sütun indeksi. |
| subtotalFunction | SubtotalFunction | Alt toplam işlevi türü. |
| subtotalColumnIndexList | Int32[] | Alt toplam yapılacak sütun indeksleri. |
| functionLabel | String | Alt toplam işlevinin etiketi. |
| grandCellStyle | GridTableItemStyle | Genel toplam satırının stili. |
| subtotalCellStyle | GridTableItemStyle | Alt toplam satırının stili. |
| numberType | NumberType | Alt toplam sonuç hücrelerinin sayı türü. |
| customString | String | Alt toplam sonuç hücrelerinin özel biçim dizesi. Null olabilir. |

### Ayrıca Bakınız

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle/)
* enum [NumberType](../../numbertype/)
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreateSubtotal(int, int, int, SubtotalFunction, int[]) {#createsubtotal}

Sayfada ara toplam oluşturur.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnNameRowIndex | Int32 | Sütun adı satırının satır indeksi. |
| dataRows | Int32 | Veri satırlarının sayısı. |
| groupByColumnIndex | Int32 | Gruplanacak sütunun sütun indeksi. |
| subtotalFunction | SubtotalFunction | Alt toplam işlevi türü. |
| subtotalColumnIndexList | Int32[] | Alt toplam yapılacak sütun indeksleri. |

### Ayrıca Bakınız

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


