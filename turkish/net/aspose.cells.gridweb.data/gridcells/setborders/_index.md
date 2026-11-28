---
title: "GridCells.SetBorders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCells yöntemi. Hücre aralığı için kenarlıkları ayarlar"
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridcells/setborders/
---
## GridCells.SetBorders method

Bir hücre aralığı için kenarlıkları ayarlar.

```csharp
public void SetBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, 
    SetBorderPosition position, WebBorderStyle borderStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Aralığın ilk satır numarası (sıfır tabanlı). |
| firstColumn | Int32 | Aralığın ilk sütun numarası (sıfır tabanlı). |
| rowNumber | Int32 | Satır sayısı. |
| columnNumber | Int32 | Sütun sayısı. |
| konum | SetBorderPosition | Kenarlık konumu. |
| borderStyle | WebBorderStyle | Kenarlık stili. |

### Örnekler

```csharp
[C#]
  GridWeb GridWeb1 = new GridWeb();
  WebBorderStyle borderStyle1 = new WebBorderStyle();
 GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### Ayrıca Bakınız

* enum [SetBorderPosition](../../../aspose.cells.gridweb/setborderposition/)
* class [WebBorderStyle](../../../aspose.cells.gridweb/webborderstyle/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


