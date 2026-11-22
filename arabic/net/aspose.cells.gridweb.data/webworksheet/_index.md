---
title: "الفئة WebWorksheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.GridWeb.Data.WebWorksheet class. يمثل ورقة عمل ويب"
type: docs
url: /ar/net/aspose.cells.gridweb.data/webworksheet/
---
## WebWorksheet class

يمثل ورقة عمل ويب.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet instead")]
public class WebWorksheet : Control, ISerializable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WebWorksheet](webworksheet/#constructor)() | منشئ WebWorksheet. |
| [WebWorksheet](webworksheet/#constructor_1)(MainWeb, GridWorksheet) | منشئ WebWorksheet. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | ربط مجموعة الأعمدة. |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | الكائن الفعلي لمصدر البيانات المرتبط في وقت التشغيل. يكون كائن DataView عندما تكون خاصية DataSource هي كائن DataSet أو DataTable أو DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | في وضع ربط البيانات، تشير BindStartRow و BindStartColumn إلى موضع الشبكة لربط مصدر البيانات. |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | في وضع ربط البيانات، تشير BindStartRow و BindStartColumn إلى موضع الشبكة لربط مصدر البيانات. |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } |  |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | يحصل على [`WebCells`](../webcells/). |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | يحصل على عدد صفوف الربط في وضع ربط البيانات. |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | يحصل أو يضبط الـ DataMember من مصدر البيانات متعدد الأعضاء. عادةً يمثل كائن DataTable من DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | يحصل أو يضبط الـ DataSource. عادةً هو كائن DataSet. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | في وضع ربط البيانات، يحدد ما إذا كان يجب إنشاء عناوين رؤوس الأعمدة المرتبطة في الورقة. |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | يحصل على مجموعة HyperlinkCollection. |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | يحصل على الفهرس الخاص به داخل أوراق العمل. |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | يحصل أو يضبط ما إذا كانت ورقة العمل محمية. عندما تكون ورقة العمل محمية، لا يمكن تعديل جميع الخلايا باستثناء الخلية التي تكون خاصية IsLocked لها false. |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | يحصل أو يضبط اسم الورقة. |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } |  |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | يحصل على مجموعة إعدادات التحقق من صحة البيانات في ورقة العمل. |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | يحدد ما إذا كان اسم هذه الورقة يُظهر في علامات تبويب الورقة في التحكم. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn)(int) | يضبط عرض العمود تلقائيًا. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | يضبط عرض العمود تلقائيًا. هذه الطريقة تضبط عرض العمود بناءً على المحتوى في نطاق من الخلايا داخل العمود من startRow إلى endRow. AutoFitColumn هي دالة غير دقيقة. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | يلغي ويحذف صف الربط المضاف حديثًا. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | يؤكد صف الربط المضاف حديثًا ويضيفه إلى مصدر البيانات. |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | ينسخ من كائن ورقة عمل آخر. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | بعد تعيين مصدر بيانات لورقة العمل، استدعِ هذه الطريقة لتوليد الأعمدة المرتبطة تلقائيًا. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | ينشئ صف ربط جديد ويربطه بمصدر البيانات. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | ينشئ مجموعًا فرعيًا في الورقة. |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | ربط الورقة بمصدر البيانات. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | يحذف صف ربط. |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | يثبت الألواح عند الخلية المحددة في ورقة العمل. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows)(int, int) | يقوم بتجميع الصفوف. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows_1)(int, int, bool) | يقوم بتجميع الصفوف. |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | يجعل جميع الخلايا قابلة للتحرير. هذه سمة موسعة. |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | يجعل جميع الخلايا للقراءة فقط. هذه سمة موسعة؛ لاحظ أن هذه السمة لا يمكن حفظها في الخلية الفعلية، إذا أردت الحفاظ على الحماية يرجى استخدام setProtect. |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | يجعل نطاقًا من الخلايا قابلاً للتحرير. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells اجعل جميع الخلايا للقراءة فقط عن طريق استدعاء طريقة SetAllCellsReadonly. ثم استدعِ هذه الطريقة لتحديد نطاق الخلايا التي يجب أن تكون قابلة للتحرير. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | يجعل نطاقًا من الخلايا للقراءة فقط. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells أولاً اجعل جميع الخلايا قابلة للتحرير عن طريق استدعاء طريقة SetAllCellsEditable. ثم استدعِ هذه الطريقة لتحديد نطاق الخلايا التي يجب أن تكون للقراءة فقط. |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | يفك تجميد الألواح في ورقة العمل. |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | يفك تجميع الصفوف. |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | يقوم بتحديث قيمة خاصية سجل مصدر البيانات المرتبط وفقًا لقيمة الخلية. |

### ملاحظات

ملاحظة: هذه الفئة الآن مهجورة. يرجى استخدام GridWorksheet بدلاً من ذلك. سيتم إزالة هذه الفئة بعد 6 أشهر منذ أغسطس 2014. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp

 [C#]
 ...
 using System.Web.UI.WebControls;
 ...
 ...

 WebWorksheets Worksheets = GridWeb1.WebWorksheets;
	WebCells cells = Worksheets[0].Cells;

	//يضبط ارتفاع الصف الافتراضي
	cells.StandardHeight = new Unit(16, UnitType.Point);
	//يضبط ارتفاع الصف
	cells.SetRowHeight(2, new Unit(20, UnitType.Point));

	//يضبط عرض العمود الافتراضي
	cells.StandardWidth = new Unit(50, UnitType.Point);
	//يضبط عرض العمود
	cells.SetColumnWidth(3, new Unit(80, UnitType.Point));

	//دمج الخلايا
	cells.Merge(5, 4, 2, 2);

	//استيراد البيانات
	DataSet1 ds1 = new DataSet1();

	for (int i =0; i<16; i++)
	{
		DataSet1.Table1Row row = ds1.Table1.NewTable1Row();
		row["c1"] = "hello1";
		row["c2"] = i;
		row["c3"] = "data";
		ds1.Table1.AddTable1Row(row);
	}

	GridWeb1.WebWorksheets.ImportDataView(ds1.Table1.DefaultView, null, null);

 //استيراد من ملف إكسل
 Worksheets.ImportExcelFile("c:\\file1.xls");

 [Visual Basic]
	Imports System.Web.UI.WebControls
	...
	...

	Dim Worksheets As WebWorksheets =  GridWeb1.WebWorksheets
	Dim cells As WebCells =  Worksheets(0).Cells

	'Sets default row height
	cells.StandardHeight = New Unit(16, UnitType.Point)
	'Sets row height
	cells.SetRowHeight(2,New Unit(20,UnitType.Point))

	'Sets default colum width
	cells.StandardWidth = New Unit(50, UnitType.Point)
	'Sets column width
	cells.SetColumnWidth(3,New Unit(80,UnitType.Point))

	'Merge cells
	cells.Merge(5, 4, 2, 2)

	'Import data
	Dim ds1 As DataSet1 =  New DataSet1()

	Dim i As Integer
	For  i = 0 To 15
		Dim row As DataSet1.Table1Row =  ds1.Table1.NewTable1Row()
		row("c1") = "hello1"
		row("c2") = i
		row("c3") = "data"
		ds1.Table1.AddTable1Row(row)
	Next

	GridWeb1.WebWorksheets.ImportDataView(ds1.Table1.DefaultView, Nothing, Nothing)

	'Import from excel file
	Worksheets.ImportExcelFile("c:\\file1.xls")
```

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


