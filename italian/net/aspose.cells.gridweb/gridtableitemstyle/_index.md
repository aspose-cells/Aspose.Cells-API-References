---
title: "Classe GridTableItemStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.GridTableItemStyle. Ereditata da System.Web.UI.WebControls.TableItemStyle. Incapsula gli stili di una WebCell"
type: docs
url: /it/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

Ereditato da System.Web.UI.WebControls.TableItemStyle. Incapsula gli stili di una WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle, ISerializable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle/)() | Costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes/) { get; set; } | Attributi dell'immagine di sfondo. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl/) { get; set; } | URL dell'immagine di sfondo. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle/) { get; set; } | Specifica lo stile del bordo inferiore della cella. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom/) { get; set; } | Ottiene o imposta il formato personalizzato, null o stringa vuota significa nessun formato personalizzato. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel/) { get; set; } | Ottiene o imposta il livello di rientro. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked/) { get; set; } | Ottiene o imposta un valore che indica se una cella può essere modificata o meno quando il foglio di lavoro è protetto. Quando il foglio è protetto e IsLocked è vero, la cella non può essere modificata. Quando il foglio è protetto e IsLocked è falso, la cella può essere modificata. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle/) { get; set; } | Specifica lo stile del bordo sinistro della cella. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype/) { get; set; } | Ottiene o imposta il formato di visualizzazione di numeri e date. I modelli di formattazione sono diversi per le varie regioni. |
| [QuotePrefix](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) { get; set; } | Indica se il valore della cella inizia con un apostrofo. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle/) { get; set; } | Specifica lo stile del bordo destro della cella. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle/) { get; set; } | Ottiene o imposta l'attributo Rotazione. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle/) { get; set; } | Specifica lo stile del bordo superiore della cella. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender/#addattributestorender_1)(HtmlTextWriter, WebControl) | Solo per uso interno. Metodo di implementazione. Non chiamare direttamente questo metodo. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom/)(Style) | Copia da un altro oggetto stile. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode/)() | Funziona come funzione hash per un tipo specifico, adatta all'uso in algoritmi di hashing e strutture dati come una tabella hash. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith/)(Style) | Unisce con un altro oggetto stile. |

### Esempi

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheetCollection sheets = GridWeb1.WorkSheets;

GridWorksheet sheet = sheets.Add("demo1");

sheet.Cells[0,0].PutValue("Demo Text");
GridTableItemStyle style = sheet.Cells[0, 0].Style;

style.Font.Size = wui.WebControls.FontUnit.Point(72);
style.Wrap = false;

style.BackColor = Color.Gray;
style.BorderStyle = wui.WebControls.BorderStyle.Solid;
style.BorderWidth = wui.WebControls.Unit.Pixel(1);
style.BorderColor = Color.Silver;
style.RightBorderStyle.BorderColor = Color.Black;
style.RightBorderStyle.BorderStyle = wui.WebControls.BorderStyle.Solid;
style.RightBorderStyle.BorderWidth = wui.WebControls.Unit.Pixel(1);
style.BottomBorderStyle.BorderColor = Color.Black;
style.BottomBorderStyle.BorderStyle = wui.WebControls.BorderStyle.Solid;
style.BottomBorderStyle.BorderWidth = wui.WebControls.Unit.Pixel(1);
sheet.Cells[0, 0].Style=style;
[Visual Basic]
Dim sheets As GridWorksheetCollection =  GridWeb1.WorkSheets
Dim sheet As GridWorksheet =  sheets(sheets.Add(__0__))

Dim cell As GridCell =  sheet.Cells(0,0)
cell.StringValue = "Demo Text"

Dim style As GridTableItemStyle = cell.GetStyle()
style.Font.Size = FontUnit.Point(72)
style.Wrap = False

style.BackColor = Color.Gray
style.BorderStyle = BorderStyle.Solid
style.BorderWidth = Unit.Pixel(1)
style.BorderColor = Color.Silver

style.RightBorderStyle.BorderColor = Color.Black
style.RightBorderStyle.BorderStyle = BorderStyle.Solid
style.RightBorderStyle.BorderWidth = Unit.Pixel(1)
style.BottomBorderStyle.BorderColor = Color.Black
style.BottomBorderStyle.BorderStyle = BorderStyle.Solid
style.BottomBorderStyle.BorderWidth = Unit.Pixel(1)
cell.SetStyle(style)
```

### Vedi anche

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


