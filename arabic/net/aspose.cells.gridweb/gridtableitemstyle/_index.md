---
title: "الفئة GridTableItemStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.GridTableItemStyle. موروثة من System.Web.UI.WebControls.TableItemStyle. تُغلف أنماط WebCell."
type: docs
url: /ar/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

موروث من System.Web.UI.WebControls.TableItemStyle. يغلف أنماط WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle, ISerializable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes/) { get; set; } | سمات صورة الخلفية. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl/) { get; set; } | عنوان URL لصورة الخلفية. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle/) { get; set; } | يحدد نمط الحد السفلي للخلية. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom/) { get; set; } | يحصل أو يعيّن التنسيق المخصص، القيم null أو السلسلة الفارغة تعني عدم وجود تنسيق مخصص. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel/) { get; set; } | يحصل أو يعيّن مستوى المسافة البادئة. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا عندما تكون ورقة العمل محمية. عندما تكون ورقة العمل محمية وتكون IsLocked صحيحة، لا يمكن تحرير الخلية. عندما تكون ورقة العمل محمية وتكون IsLocked خاطئة، يمكن تحرير الخلية. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle/) { get; set; } | يحدد نمط الحد الأيسر للخلية. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype/) { get; set; } | يحصل على تنسيق العرض للأرقام والتواريخ أو يضبطه. أنماط التنسيق تختلف بين المناطق المختلفة. |
| [QuotePrefix](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) { get; set; } | يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle/) { get; set; } | يحدد نمط الحد الأيمن للخلية. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle/) { get; set; } | يحصل أو يعيّن سمة الدوران. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle/) { get; set; } | يحدد نمط الحد العلوي للخلية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender/#addattributestorender_1)(HtmlTextWriter, WebControl) | للاستخدام الداخلي فقط. طريقة تنفيذية لا تستدعِ هذه الطريقة مباشرة. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom/)(Style) | ينسخ من كائن نمط آخر. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode/)() | يعمل كدالة تجزئة لنوع معين، مناسبة للاستخدام في خوارزميات التجزئة وهياكل البيانات مثل جدول التجزئة. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith/)(Style) | يدمج مع كائن نمط آخر. |

### أمثلة

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

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


