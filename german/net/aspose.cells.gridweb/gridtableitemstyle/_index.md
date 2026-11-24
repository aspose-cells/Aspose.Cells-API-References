---
title: "Klasse GridTableItemStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.GridTableItemStyle Klasse. Erbt von System.Web.UI.WebControls.TableItemStyle. Kapselt die Stile einer WebCell."
type: docs
url: /de/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

Erbt von System.Web.UI.WebControls.TableItemStyle. Kapselt die Stile einer WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle, ISerializable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle/)() | Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes/) { get; set; } | Attribute des Hintergrundbildes. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl/) { get; set; } | URL des Hintergrundbildes. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle/) { get; set; } | Gibt den Stil des unteren Rands der Zelle an. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom/) { get; set; } | Liest oder setzt das benutzerdefinierte Format; null oder eine leere Zeichenfolge bedeutet kein benutzerdefiniertes Format. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel/) { get; set; } | Liest oder setzt die Einzugsebene. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob eine Zelle geändert werden kann, wenn das Arbeitsblatt geschützt ist. Ist das Arbeitsblatt geschützt und IsLocked ist true, kann die Zelle nicht bearbeitet werden. Ist das Arbeitsblatt geschützt und IsLocked ist false, kann die Zelle bearbeitet werden. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle/) { get; set; } | Gibt den Stil des linken Rands der Zelle an. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype/) { get; set; } | Liest oder setzt das Anzeigeformat von Zahlen und Daten. Die Formatierungsmuster unterscheiden sich je nach Region. |
| [QuotePrefix](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) { get; set; } | Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle/) { get; set; } | Gibt den Stil des rechten Rands der Zelle an. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle/) { get; set; } | Liest oder setzt das Rotationsattribut. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle/) { get; set; } | Gibt den Stil des oberen Rands der Zelle an. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender/#addattributestorender_1)(HtmlTextWriter, WebControl) | Nur für den internen Gebrauch. Implementierungsmethode. Rufen Sie diese Methode nicht direkt auf. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom/)(Style) | Kopiert von einem anderen Stilobjekt. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode/)() | Dient als Hash-Funktion für einen bestimmten Typ, geeignet für den Einsatz in Hash-Algorithmen und Datenstrukturen wie einer Hashtabelle. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith/)(Style) | Führt mit einem anderen Stilobjekt zusammen. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


