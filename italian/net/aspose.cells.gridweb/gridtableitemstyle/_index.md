---
title: GridTableItemStyle
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Ereditato da System.Web.UI.WebControls.TableItemStyle. Incapsula gli stili di un WebCell.
type: docs
weight: 780
url: /it/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

Ereditato da System.Web.UI.WebControls.TableItemStyle. Incapsula gli stili di un WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle)() | Costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes) { get; set; } | Attributi dell'immagine di sfondo. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl) { get; set; } | URL immagine di sfondo. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle) { get; set; } | Specifica lo stile del bordo inferiore della cella. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom) { get; set; } | Ottiene o imposta il formato personalizzato, stringa nulla o vuota significa nessun formato personalizzato. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel) { get; set; } | Ottiene o imposta il livello di rientro. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked) { get; set; } | Ottiene o imposta un valore che indica se una cella può essere modificata o meno quando il relativo foglio di lavoro è protetto. Quando il relativo foglio di lavoro è protetto e IsLocked è true, la cella non può essere modificata. Quando il suo foglio di lavoro è protetto e IsLocked è falso, la cella può essere modificata. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle) { get; set; } | Specifica lo stile del bordo sinistro della cella. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype) { get; set; } | Ottiene o imposta il formato di visualizzazione di numeri e date. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle) { get; set; } | Specifica lo stile del bordo destro della cella. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle) { get; set; } | Ottiene o imposta l'attributo di rotazione. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle) { get; set; } | Specifica lo stile del bordo superiore della cella. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender#addattributestorender_1)(HtmlTextWriter, WebControl) | Solo uso interno. Metodo di implementazione Non chiamare questo metodo direttamente. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom)(Style) | Copia da un altro oggetto di stile. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode)() | Serve come funzione hash per un tipo particolare, adatta per l'uso in algoritmi di hash e strutture di dati come una tabella hash. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith)(Style) | Si unisce a un altro oggetto di stile. |

### Esempi

```csharp
[C#]
...
using System.Web.UI.WebControls;
...
...
WebWorksheets sheets = GridWeb1.WebWorksheets;
sheets.Clear();
WebWorksheet sheet = sheets[sheets.Add("demo1")];

WebCell cell = sheet.Cells[0,0];
cell.StringValue = "Demo Text";

Aspose.Cells.GridWeb.TableItemStyle style = cell.GetStyle();
style.Font.Size = new FontUnit("72pt");
style.Wrap = false;

style.BackColor = Color.Gray;
style.BorderStyle = BorderStyle.Solid;
style.BorderWidth = new Unit(1, UnitType.Pixel);
style.BorderColor = Color.Silver;

style.RightBorderStyle.BorderColor = Color.Black;
style.RightBorderStyle.BorderStyle = BorderStyle.Solid;
style.RightBorderStyle.BorderWidth = new Unit(1, UnitType.Pixel);
style.BottomBorderStyle.BorderColor = Color.Black;
style.BottomBorderStyle.BorderStyle = BorderStyle.Solid;
style.BottomBorderStyle.BorderWidth = new Unit(1, UnitType.Pixel);
cell.SetStyle(style);

[Visual Basic]
...
Imports System.Web.UI.WebControls
...
...
Dim sheets As WebWorksheets =  GridWeb1.WebWorksheets
sheets.Clear()
Dim sheet As WebWorksheet =  sheets(sheets.Add(__0__))

Dim cell As WebCell =  sheet.Cells(0,0)
cell.StringValue = "Demo Text"

Dim style As Aspose.Cells.GridWeb.TableItemStyle = cell.GetStyle()
style.Font.Size = New FontUnit("72pt")
style.Wrap = False

style.BackColor = Color.Gray
style.BorderStyle = BorderStyle.Solid
style.BorderWidth = New Unit(1, UnitType.Pixel)
style.BorderColor = Color.Silver

style.RightBorderStyle.BorderColor = Color.Black
style.RightBorderStyle.BorderStyle = BorderStyle.Solid
style.RightBorderStyle.BorderWidth = New Unit(1, UnitType.Pixel)
style.BottomBorderStyle.BorderColor = Color.Black
style.BottomBorderStyle.BorderStyle = BorderStyle.Solid
style.BottomBorderStyle.BorderWidth = New Unit(1, UnitType.Pixel)
cell.SetStyle(style)
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* assemblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
