---
title: "GridCells.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCells özelliği. Belirtilen hücre satır indeksi ve sütun indeksindeki GridCell öğesini alır"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridcells/item/
---
## GridCells indexer (1 of 2)

Belirtilen hücre satır indeksi ve sütun indeksindeki [`GridCell`](../../gridcell/) öğesini alır.

```csharp
public GridCell this[int row, int column] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| satır | Satır indeksi. |
| sütun | Sütun indeksi. |

### Dönüş Değeri

Bu [`GridCell`](../../gridcell/) nesnesi.

### Örnekler

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### Ayrıca Bakınız

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridCells indexer (2 of 2)

Belirtilen hücre adındaki [`GridCell`](../../gridcell/) öğesini alır.

```csharp
public GridCell this[string cellName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| cellName | Hücre adı, sütun harfi ve satır numarası dahil, örneğin A5. |

### Dönüş Değeri

Bir [`GridCell`](../../gridcell/) nesnesi

### Ayrıca Bakınız

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


