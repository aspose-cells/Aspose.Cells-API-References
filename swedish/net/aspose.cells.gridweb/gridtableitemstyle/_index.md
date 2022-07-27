---
title: GridTableItemStyle
second_title: Aspose.Cells för .NET API-referens
description: Ärvt från System.Web.UI.WebControls.TableItemStyle. Kapslar in stilarna för en WebCell.
type: docs
weight: 780
url: /sv/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

Ärvt från System.Web.UI.WebControls.TableItemStyle. Kapslar in stilarna för en WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle)() | Standardkonstruktor. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes) { get; set; } | Attribut för bakgrundsbild. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl) { get; set; } | Bakgrundsbildens url. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle) { get; set; } | Anger stilen för cellens nedre kant. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom) { get; set; } | Hämtar eller ställer in det anpassade formatet, null eller tom sträng betyder inget anpassat format. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel) { get; set; } | Hämtar eller ställer in indragsnivå. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked) { get; set; } | Hämtar eller ställer in ett värde som anger om en cell kan ändras eller inte när dess kalkylblad är skyddat. När dess kalkylblad är skyddat och IsLocked är sant, kan cellen inte redigeras. När dess kalkylblad är skyddat och IsLocked är falskt kan cellen redigeras. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle) { get; set; } | Anger stilen för cellens vänstra kantlinje. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype) { get; set; } | Hämtar eller ställer in visningsformat för siffror och datum. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle) { get; set; } | Anger stilen för cellens högra kantlinje. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle) { get; set; } | Hämtar eller ställer in rotationsattribut. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle) { get; set; } | Anger stilen för cellens övre kant. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender#addattributestorender_1)(HtmlTextWriter, WebControl) | Endast intern användning. Implementeringsmetod Anrop inte denna metod direkt. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom)(Style) | Kopierar från ett annat stilobjekt. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode)() | Fungerar som en hashfunktion för en viss typ, lämplig för användning i hashalgoritmer och datastrukturer som en hashtabell. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith)(Style) | Slås samman med ett annat stilobjekt. |

### Exempel

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

### Se även

* namnutrymme [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* hopsättning [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
