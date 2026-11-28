---
title: "GridCells.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCells özelliği. Belirtilen hücre satır indeksi ve sütun indeksindeki GridCell öğesini alır"
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridcells/item/
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
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.WorkSheets[0].Cells;
//A1 hücresini alır
GridCell cell = cells[0, 0];	

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
 'Gets the cell at "A1"
Dim cell As Cell =  cells(0,0) 
```

### Ayrıca Bakınız

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

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

### Örnekler

```csharp
[C#]
ridWeb GridWeb1 = new GridWeb();
 GridCells cells = GridWeb1.WorkSheets[0].Cells;
 GridCell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Ayrıca Bakınız

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


