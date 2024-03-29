---
title: WebBorderStyle
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula lo stile della tabella Web o del bordo della cella.
type: docs
weight: 930
url: /it/net/aspose.cells.gridweb/webborderstyle/
---
## WebBorderStyle class

Incapsula lo stile della tabella Web o del bordo della cella.

```csharp
public class WebBorderStyle
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WebBorderStyle](webborderstyle)() | Costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BorderColor](../../aspose.cells.gridweb/webborderstyle/bordercolor) { get; set; } | Ottiene o imposta il colore del bordo. Fare riferimento a System.Drawing.Color struct. |
| [BorderStyle](../../aspose.cells.gridweb/webborderstyle/borderstyle) { get; set; } | Ottiene o imposta lo stile del bordo. Fare riferimento al documento .NET SDK su System.Web.UI.WebControls.BorderStyle enum. |
| [BorderWidth](../../aspose.cells.gridweb/webborderstyle/borderwidth) { get; set; } | Ottiene o imposta la larghezza del bordo. Fare riferimento a System.Web.UI.WebControls.Unit struct. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CopyFrom](../../aspose.cells.gridweb/webborderstyle/copyfrom)(WebBorderStyle) | Copia da un altro oggetto di stile. |
| override [GetHashCode](../../aspose.cells.gridweb/webborderstyle/gethashcode)() |  |

### Osservazioni

Fare riferimento al documento .NET SDK per ulteriori informazioni sullo spazio dei nomi System.Web.UI.WebControls.

### Esempi

```csharp
[C#]
	WebCell cell1 = GridWeb1.WebWorksheets[0].Cells["A1"];
	cell1.Style.LeftBorderStyle.BorderColor = System.Drawing.Color.Red;
	cell1.Style.LeftBorderStyle.BorderStyle = System.Web.UI.WebControls.BorderStyle.Solid;
	cell1.Style.LeftBorderStyle.BorderWidth = new System.Web.UI.WebControls.Unit(16, System.Web.UI.WebControls.UnitType.Point);

[Visual Basic]
	Dim cell1 As WebCell =  GridWeb1.WebWorksheets(0).Cells("A1")
	cell1.Style.LeftBorderStyle.BorderColor = System.Drawing.Color.Red
	cell1.Style.LeftBorderStyle.BorderStyle = System.Web.UI.WebControls.BorderStyle.Solid
	cell1.Style.LeftBorderStyle.BorderWidth = New System.Web.UI.WebControls.Unit(16, System.Web.UI.WebControls.UnitType.Point)
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* assemblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
