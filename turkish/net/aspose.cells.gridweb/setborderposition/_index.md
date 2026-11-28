---
title: "Enum SetBorderPosition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.SetBorderPosition enum'ı. Hücre aralığının ayarlanacak kenar konumunu temsil eder"
type: docs
url: /tr/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

Bir hücre aralığının ayarlanacak kenarlık konumunu temsil eder.

```csharp
public enum SetBorderPosition
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Top | `0` | Üst kenar |
| Bottom | `1` | Alt kenar |
| Left | `2` | Sol kenar |
| Right | `3` | Sağ kenar |
| HorizontalMiddle | `4` | Alt kenar |
| VerticalMiddle | `5` | YatayOrta kenarlar |
| Outline | `6` | VerticalMiddle kenarlıklar |
| Cross | `7` | Çapraz kenarlıklar |
| None | `8` | Kenarlık yok |

### Örnekler

```csharp
[C#]
    GridWeb GridWeb1=new GridWeb();
	GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle);

[VB]
	GridWeb1.WorkSheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle)
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


