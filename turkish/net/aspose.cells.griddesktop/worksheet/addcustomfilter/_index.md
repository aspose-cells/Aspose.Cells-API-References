---
title: "Worksheet.AddCustomFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Belirtilen satır aralığı için başlangıç satırından bitiş satırına özel filtre ekle."
type: docs
url: /tr/net/aspose.cells.griddesktop/worksheet/addcustomfilter/
---
## AddCustomFilter(int, int, object[], GridFilterOperatorType[]) {#addcustomfilter}

Başlangıç satırından bitiş satırına kadar belirtilen satır aralığı için özel filtre ekler.

```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras, 
    GridFilterOperatorType[] filterOperatorTypes)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startrow | Int32 | Filtre aralığının startrow değeri |
| startcolumn | Int32 | Filtre aralığının startcolumn değeri |
| critiras | Object[] | Sütunlar için critira dizisi, her biri her sütuna uygulanır. |
| filterOperatorTypes | GridFilterOperatorType[] | Sütunlar için filtre işlem tipi dizisi, her biri her sütuna uygulanır. |

### Ayrıca Bakınız

* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## AddCustomFilter(int, string) {#addcustomfilter_1}

Belirtilen satır için özel filtre ekle.

```csharp
public void AddCustomFilter(int row, string critira)
```

### Açıklamalar

Filtre kriterleri dizesi. , ve ; karakterlerini ayırıcı olarak kullandığımızı unutmayın, bu yüzden hücre değeri bu ayırıcıları içermemelidir. Aşağıda kriter dizesi örnekleri verilmiştir: //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


