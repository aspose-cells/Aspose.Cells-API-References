---
title: "Sınıf GridTableItemStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.GridTableItemStyle sınıfı. System.Web.UI.WebControls.TableItemStyle sınıfından türetilmiştir. Bir WebCell'in stillerini kapsüller"
type: docs
url: /tr/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

System.Web.UI.WebControls.TableItemStyle sınıfından kalıtılmıştır. Bir WebCell'in stillerini kapsar.

```csharp
public class GridTableItemStyle : TableItemStyle, ISerializable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes/) { get; set; } | Arka plan görüntüsü özellikleri. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl/) { get; set; } | Arka plan görüntüsü URL'si. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle/) { get; set; } | Hücrenin alt kenarlık stilini belirtir. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom/) { get; set; } | Özel biçimi alır veya ayarlar, null veya boş dize özel biçim olmadığı anlamına gelir. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel/) { get; set; } | Girinti seviyesini alır veya ayarlar. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked/) { get; set; } | Çalışma sayfası korunduğunda bir hücrenin değiştirilebilir olup olmadığını gösteren bir değeri alır veya ayarlar. Çalışma sayfası korunduğunda ve IsLocked true ise hücre düzenlenemez. Çalışma sayfası korunduğunda ve IsLocked false ise hücre düzenlenebilir. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle/) { get; set; } | Hücrenin sol kenarlık stilini belirtir. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype/) { get; set; } | Sayıların ve tarihlerin görüntüleme biçimini alır veya ayarlar. Biçimlendirme desenleri farklı bölgeler için farklıdır. |
| [QuotePrefix](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) { get; set; } | Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle/) { get; set; } | Hücrenin sağ kenarlık stilini belirtir. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle/) { get; set; } | Dönme özelliğini alır veya ayarlar. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle/) { get; set; } | Hücrenin üst kenarlık stilini belirtir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender/#addattributestorender_1)(HtmlTextWriter, WebControl) | Yalnızca dahili kullanım içindir. Uygulama yöntemi, bu yöntemi doğrudan çağırmayın. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom/)(Style) | Başka bir stil nesnesinden kopyalar. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode/)() | Belirli bir tip için bir hash işlevi olarak hizmet verir, hash tabloları gibi hash algoritmaları ve veri yapılarında kullanılmaya uygundur. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith/)(Style) | Başka bir stil nesnesiyle birleştirir. |

### Örnekler

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

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


