---
title: GridTableItemStyle
second_title: Aspose.Cells für .NET-API-Referenz
description: geerbt von System.Web.UI.WebControls.TableItemStyle. Kapselt die Stile einer WebCell.
type: docs
weight: 780
url: /de/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

geerbt von System.Web.UI.WebControls.TableItemStyle. Kapselt die Stile einer WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle)() | Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes) { get; set; } | Hintergrundbildattribute. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl) { get; set; } | Hintergrundbild-URL. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle) { get; set; } | Gibt den Stil des unteren Rahmens der Zelle an. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom) { get; set; } | Ruft das benutzerdefinierte Format ab oder legt es fest, null oder leere Zeichenfolge bedeutet kein benutzerdefiniertes Format. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel) { get; set; } | Ruft die Einzugsebene ab oder legt sie fest. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob eine Zelle geändert werden kann oder nicht, wenn ihr Arbeitsblatt geschützt ist. Wenn ihr Arbeitsblatt geschützt ist und IsLocked wahr ist, kann die Zelle nicht bearbeitet werden. Wenn das Arbeitsblatt is protected und IsLocked false ist, kann die Zelle bearbeitet werden. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle) { get; set; } | Gibt den Stil des linken Rahmens der Zelle an. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype) { get; set; } | Ruft das Anzeigeformat von Zahlen und Daten ab oder legt es fest. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle) { get; set; } | Gibt den Stil des rechten Rahmens der Zelle an. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle) { get; set; } | Ruft das Rotationsattribut ab oder legt es fest. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle) { get; set; } | Gibt den Stil des oberen Rahmens der Zelle an. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender#addattributestorender_1)(HtmlTextWriter, WebControl) | Nur zur internen Verwendung. Implementierungsmethode Rufen Sie diese Methode nicht direkt auf. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom)(Style) | Kopien von einem anderen Stilobjekt. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode)() | Dient als Hash-Funktion für einen bestimmten Typ, geeignet für die Verwendung in Hash-Algorithmen und Datenstrukturen wie einer Hash-Tabelle. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith)(Style) | Wird mit einem anderen Stilobjekt zusammengeführt. |

### Beispiele

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

### Siehe auch

* namensraum [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* Montage [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
