---
title: "WebCells.SetBorders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebCells-Methode. Setzt Rahmen für einen Zellenbereich."
type: docs
url: /de/net/aspose.cells.gridweb.data/webcells/setborders/
---
## WebCells.SetBorders method

Setzt Rahmen für einen Zellenbereich.

```csharp
public void SetBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, 
    SetBorderPosition position, WebBorderStyle borderStyle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Die erste Zeilennummer des Bereichs(nullbasiert). |
| firstColumn | Int32 | Die erste Spaltennummer des Bereichs(nullbasiert). |
| rowNumber | Int32 | Die Zeilenzahl. |
| columnNumber | Int32 | Die Spaltenzahl. |
| Position | SetBorderPosition | Die Rahmenposition. |
| borderStyle | WebBorderStyle | Der Randstil. |

### Beispiele

```csharp
[C#]
	GridWeb1.WebWorksheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### Siehe auch

* enum [SetBorderPosition](../../../aspose.cells.gridweb/setborderposition/)
* class [WebBorderStyle](../../../aspose.cells.gridweb/webborderstyle/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


