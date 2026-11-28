---
title: "WebCells.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebCells özelliği. Belirtilen hücre satır indeksi ve sütun indeksindeki Cell öğesini alır."
type: docs
url: /tr/net/aspose.cells.gridweb.data/webcells/item/
---
## WebCells indexer (1 of 2)

Belirtilen hücre satır indeksi ve sütun indeksindeki Cell öğesini alır.

```csharp
public WebCell this[int row, int column] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| satır | Satır indeksi. |
| sütun | Sütun indeksi. |

### Dönüş Değeri

Cell nesnesi.

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

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## WebCells indexer (2 of 2)

Belirtilen hücre adındaki Cell öğesini alır.

```csharp
public WebCell this[string cellName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| cellName | Hücre adı, sütun harfi ve satır numarası dahil, örneğin A5. |

### Dönüş Değeri

Bir Cell nesnesi

### Örnekler

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Ayrıca Bakınız

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


