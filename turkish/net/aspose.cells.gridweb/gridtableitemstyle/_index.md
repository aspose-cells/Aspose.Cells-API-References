---
title: GridTableItemStyle
second_title: Aspose.Cells for .NET API Referansı
description: System.Web.UI.WebControls.TableItemStyle. öğesinden devralındı Bir WebCellin stillerini kapsüller.
type: docs
weight: 780
url: /tr/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

System.Web.UI.WebControls.TableItemStyle. öğesinden devralındı Bir WebCell'in stillerini kapsüller.

```csharp
public class GridTableItemStyle : TableItemStyle
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle)() | Varsayılan yapıcı. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes) { get; set; } | Arka plan resmi öznitelikleri. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl) { get; set; } | Arka plan resmi url. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle) { get; set; } | Hücrenin alt kenarlığının stilini belirtir. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom) { get; set; } | Özel biçimi alır veya ayarlar, boş veya boş dize, özel biçim olmadığı anlamına gelir. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel) { get; set; } | Girinti düzeyini alır veya ayarlar. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked) { get; set; } | Çalışma sayfası korumalıyken bir hücrenin değiştirilip değiştirilemeyeceğini belirten bir değer alır veya ayarlar. Çalışma sayfası korumalıysa ve IsLocked true olduğunda, hücre düzenlenemez. Çalışma sayfası is korumalı ve IsLocked false olduğunda, hücre düzenlenebilir. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle) { get; set; } | Hücrenin sol kenarlığının stilini belirtir. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype) { get; set; } | Sayıların ve tarihlerin görüntülenme biçimini alır veya ayarlar. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle) { get; set; } | Hücrenin sağ kenarlığının stilini belirtir. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle) { get; set; } | Döndürme özniteliğini alır veya ayarlar. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle) { get; set; } | Hücrenin üst kenarlığının stilini belirtir. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender#addattributestorender_1)(HtmlTextWriter, WebControl) | Yalnızca dahili kullanım. Uygulama yöntemi Bu yöntemi doğrudan çağırmayın. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom)(Style) | Başka bir stil nesnesinden kopyalar. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode)() | Karma algoritmalarında ve karma tablosu gibi veri yapılarında kullanıma uygun, belirli bir tür için karma işlevi olarak hizmet eder. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith)(Style) | Başka bir stil nesnesiyle birleşir. |

### Örnekler

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

### Ayrıca bakınız

* ad alanı [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* toplantı [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
