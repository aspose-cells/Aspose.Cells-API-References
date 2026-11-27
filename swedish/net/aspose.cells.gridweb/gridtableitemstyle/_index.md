---
title: "Klass GridTableItemStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.GridTableItemStyle-klass. Ärvd från System.Web.UI.WebControls.TableItemStyle. Inkapslar stilarna för en WebCell."
type: docs
url: /sv/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

Arv från System.Web.UI.WebControls.TableItemStyle. Inkapslar stilarna för en WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle, ISerializable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle/)() | Standardkonstruktor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes/) { get; set; } | Bakgrundsbildsattribut. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl/) { get; set; } | Bakgrundsbild-URL. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle/) { get; set; } | Anger stil för cellens nedre kant. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom/) { get; set; } | Hämtar eller anger det anpassade formatet, null eller tom sträng betyder inget anpassat format. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel/) { get; set; } | Hämtar eller anger indenteringsnivå. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked/) { get; set; } | Hämtar eller anger ett värde som indikerar om en cell kan ändras eller inte när dess kalkylblad är skyddat. När kalkylbladet är skyddat och IsLocked är true, kan cellen inte redigeras. När kalkylbladet är skyddat och IsLocked är false, kan cellen redigeras. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle/) { get; set; } | Anger stil för cellens vänstra kant. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype/) { get; set; } | Hämtar eller anger visningsformatet för tal och datum. Formateringsmönstren skiljer sig åt mellan olika regioner. |
| [QuotePrefix](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) { get; set; } | Indikerar om cellens värde börjar med enkelfnutt. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle/) { get; set; } | Anger stil för cellens högra kant. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle/) { get; set; } | Hämtar eller anger rotationsattributet. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle/) { get; set; } | Anger stil för cellens övre kant. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender/#addattributestorender_1)(HtmlTextWriter, WebControl) | Endast för internt bruk. Implementationsmetod. Anropa inte denna metod direkt. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom/)(Style) | Kopierar från ett annat stilobjekt. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode/)() | Fungerar som en hashfunktion för en viss typ, lämplig för användning i hashalgoritmer och datastrukturer som en hashtabell. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith/)(Style) | Slår samman med ett annat stilobjekt. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


