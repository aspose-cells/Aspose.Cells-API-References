---
title: "WebCells.SetBorders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WebCells. Imposta i bordi per un intervallo di celle"
type: docs
url: /it/net/aspose.cells.gridweb.data/webcells/setborders/
---
## WebCells.SetBorders method

Imposta i bordi per un intervallo di celle.

```csharp
public void SetBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, 
    SetBorderPosition position, WebBorderStyle borderStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Il numero della prima riga dell'intervallo (basato su zero). |
| firstColumn | Int32 | Il numero della prima colonna dell'intervallo (basato su zero). |
| rowNumber | Int32 | Il numero di righe. |
| columnNumber | Int32 | Il numero di colonne. |
| posizione | SetBorderPosition | La posizione del bordo. |
| borderStyle | WebBorderStyle | Lo stile del bordo. |

### Esempi

```csharp
[C#]
	GridWeb1.WebWorksheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### Vedi anche

* enum [SetBorderPosition](../../../aspose.cells.gridweb/setborderposition/)
* class [WebBorderStyle](../../../aspose.cells.gridweb/webborderstyle/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


