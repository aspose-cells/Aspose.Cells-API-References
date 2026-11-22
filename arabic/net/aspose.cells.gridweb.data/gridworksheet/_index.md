---
title: "Class GridWorksheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.GridWeb.Data.GridWorksheet class. يغلف الكائن الذي يمثل ورقة عمل واحدة"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridworksheet/
---
## GridWorksheet class

يحتوي على الكائن الذي يمثل ورقة عمل واحدة.

```csharp
public class GridWorksheet : Control, ISerializable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell/) { get; set; } | يحصل أو يعيّن الخلية النشطة في ورقة العمل. |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage/) { get; set; } | يحصل أو يعيّن صورة خلفية ورقة العمل. |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns/) { get; } | ربط مجموعة الأعمدة. |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource/) { get; } | الكائن الفعلي لمصدر البيانات المرتبط في وقت التشغيل. يكون كائن DataView عندما تكون خاصية DataSource هي كائن DataSet أو DataTable أو DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn/) { get; set; } | في وضع ربط البيانات، تشير BindStartRow و BindStartColumn إلى موضع الشبكة لربط مصدر البيانات. |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow/) { get; set; } | في وضع ربط البيانات، تشير BindStartRow و BindStartColumn إلى موضع الشبكة لربط مصدر البيانات. |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells/) { get; } | يحصل على مجموعة [`GridCell`](../gridcell/). |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename/) { get; } | يمثل اسم رمز ورقة العمل. |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments/) { get; } | يحصل على مجموعة [`GridComment`](../gridcomment/). |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows/) { get; set; } | يحصل على عدد صفوف الربط في وضع ربط البيانات. |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember/) { get; set; } | يحصل أو يضبط الـ DataMember من مصدر البيانات متعدد الأعضاء. عادةً يمثل كائن DataTable من DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource/) { get; set; } | يحصل أو يضبط الـ DataSource. عادةً هو كائن DataSet. |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft/) { get; set; } | يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. القيمة الافتراضية هي false. |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros/) { get; set; } | صحيح إذا تم عرض القيم الصفرية. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader/) { get; set; } | في وضع ربط البيانات، يحدد ما إذا كان يجب إنشاء عناوين رؤوس الأعمدة المرتبطة في الورقة. |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn/) { get; set; } | يمثل فهرس العمود الأول الظاهر. |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow/) { get; set; } | يمثل فهرس الصف الأول الظاهر. |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell/) { get; set; } | يحصل أو يعيّن الخلية النشطة في ورقة العمل. |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks/) { get; } | يحصل على مجموعة [`GridHyperlinkCollection`](../gridhyperlinkcollection/). |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index/) { get; } | يحصل على فهرس الورقة في مجموعة أوراق العمل. |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true. |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow/) { get; set; } | يشير إلى ما إذا كان سيتم وضع صف الملخص أسفل صفوف التفاصيل في المخطط. |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name/) { get; set; } | يحصل على أو يضبط اسم ورقة العمل. |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown/) { get; set; } | يحدد ما إذا كان يتم إظهار المخطط. |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures/) { get; } | يحصل على مجموعة [`Pictures`](./pictures/). |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables/) { get; } | يحصل على الـ pivotTables في ورقة العمل. |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected/) { get; set; } | يشير إلى ما إذا تم اختيار ورقة العمل هذه عند فتح المصنف. |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes/) { get; } | يحصل على مجموعة [`Pictures`](./pictures/). |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight/) { get; set; } | يحصل أو يضبط ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة النقاط. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels/) { get; set; } | يحصل أو يضبط ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة البكسل. |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor/) { get; set; } | يمثل لون تبويب ورقة العمل. |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations/) { get; } | يحصل على مجموعة إعدادات التحقق من صحة البيانات في ورقة العمل. |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible/) { get; set; } | يحدد ما إذا كان اسم هذه الورقة يُظهر في علامات تبويب الورقة في التحكم. |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook/) { get; } | يحصل على كائن [`GridWorkbook`](../gridworkbook/) من مجموعة أوراق العمل. |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom/) { get; set; } | يمثل عامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter/)(int, int, int) | يحدد النطاق الذي ينطبق عليه AutoFilter المحدد. |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter/)(int, string) | أضف مرشحًا مخصصًا للصف المحدد. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn)(int) | يضبط عرض العمود تلقائيًا. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | يضبط عرض العمود تلقائيًا. |
| [AutoFitColumns](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumns/)() |  |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow)(int) | يضبط ارتفاع الصف تلقائيًا. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_1)(int, int, int) | يضبط ارتفاع الصف تلقائيًا. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_2)(int, int, int, int) | يضبط ارتفاع الصف في نطاق مستطيل تلقائيًا. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows)() | يضبط جميع الصفوف في هذه ورقة العمل تلقائيًا. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_1)(bool) | يضبط جميع الصفوف في هذه ورقة العمل تلقائيًا. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_2)(int, int) | يضبط ارتفاع الصف في نطاق تلقائيًا. |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula/)(string) | يحسب صيغة. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow/)() | يلغي ويحذف صف الربط المضاف حديثًا. |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments/)() | يمسح جميع التعليقات في جدول البيانات المصمم. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow/)() | يؤكد صف الربط المضاف حديثًا ويضيفه إلى مصدر البيانات. |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy/)(GridWorksheet) | ينسخ المحتويات والتنسيقات من ورقة عمل أخرى. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns/)() | بعد تعيين مصدر بيانات لورقة العمل، استدعِ هذه الطريقة لتوليد الأعمدة المرتبطة تلقائيًا. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow/)() | ينشئ صف ربط جديد ويربطه بمصدر البيانات. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal)(int, int, int, SubtotalFunction, int[]) | ينشئ مجموعًا فرعيًا في الورقة. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | ينشئ مجموعًا فرعيًا في الورقة. |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind/)() | ربط الورقة بمصدر البيانات. |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate/)(AccessDataSource) | ربط الورقة بمصدر البيانات. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow/)(int) | يحذف صف ربط. |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring/)(int, string) | يضبط الفلتر للعمود. لاحظ أننا سنستدعي AddAutoFilter قبل استدعاء filterString. سلسلة معايير الفلتر. لاحظ أننا نستخدم الفاصلة-&gt;"," كحرف تقسيم، لذا يجب ألا تحتوي قيمة الخلية التي تريد تصفيتها على الفاصلة. filterString(10,"123,456") يعني أن العمود 10 يجب أن يحتوي على 123 أو 456، filterString(10,"123") يعني أن العمود 10 يجب أن يحتوي على 123 قيمة فهرس العمود مقسمة بالفاصلة، مثال: 123,456,789 أو abc |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes_1)(string, int, int) | يثبت الألواح عند الخلية المحددة في ورقة العمل. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes)(int, int, int, int) | يثبت الألواح عند الخلية المحددة في ورقة العمل. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption/)(int) | يحصل على تسمية العمود. إذا لم يتم تعيين التسمية، يرجع سلسلة فارغة. |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip/)(int) | يحصل على نص تلميح أداة رأس العمود. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly/)(int) | يحصل على ما إذا كان العمود للقراءة فقط. هذه طريقة موسعة من GridWeb تحديدًا، لن تُحفظ أو تُؤثر في ملف Excel الفعلي. |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes/)(out int, out int, out int, out int) | يحصل على تجميد الألواح. |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly/)(int, int) | يحصل على ما إذا كانت الخلية للقراءة فقط. هذه خاصية موسعة من GridWeb، لن تُحفظ في ملف Excel الفعلي. |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption/)(int) | يحصل على تسمية الصف. إذا لم يتم تعيين التسمية، يرجع سلسلة فارغة. |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip/)(int) | يحصل على نص تلميح رأس الصف. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly/)(int) | يحصل على ما إذا كان الصف للقراءة فقط. هذه طريقة موسعة من GridWeb تحديدًا، لن تُحفظ ولن تؤثر في ملف Excel الفعلي. |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows/)(int, int, bool) | يقوم بتجميع الصفوف. |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected/)() | يشير إلى ما إذا كانت ورقة العمل محمية. |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto/)(int) | ينقل الورقة إلى موقع آخر في جدول البيانات. |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter/)() | تحديث الفلاتر التلقائية لإخفاء أو إظهار الصفوف. |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter/)() | إزالة الفلتر التلقائي للورقة. |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal/)() | يزيل المجموع الفرعي الذي تم إنشاؤه بواسطة طريقة CreateSubtotal في الورقة. |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter/)(int) | الإزاحة الصحيحة للحقول التي تريد تطبيقها، بناءً على أول عمود تصفية (من يسار القائمة؛ الحقل الأيسر هو الحقل 0). |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable/)() | يجعل جميع الخلايا قابلة للتحرير. هذه سمة موسعة. |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly/)() | يجعل جميع الخلايا للقراءة فقط. هذه سمة موسعة؛ لاحظ أن هذه السمة لا يمكن حفظها في الخلية الفعلية، إذا أردت الحفاظ على الحماية يرجى استخدام setProtect. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption/)(int, string) | يضبط التسمية للعمود. يرجى ملاحظة أن هذه سمة امتداد ولا يمكن حفظها في ملف Excel. |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip/)(int, string) | يضبط نص تلميح رأس العمود. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly/)(int, bool) | يضبط عمودًا للقراءة فقط بحيث لا يستطيع المستخدم حذفه من جانب العميل. هذه طريقة موسعة من GridWeb تحديدًا، لن تُحفظ ولن تؤثر في ملف Excel الفعلي. |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange/)(int, int, int, int) | يجعل نطاقًا من الخلايا قابلاً للتحرير. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells اجعل جميع الخلايا للقراءة فقط عن طريق استدعاء طريقة SetAllCellsReadonly. ثم استدعِ هذه الطريقة لتحديد نطاق الخلايا التي يجب أن تكون قابلة للتحرير. |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly/)(int, int, bool) | يضبط ما إذا كانت الخلية للقراءة فقط. هذه سمة موسعة من GridWeb، لن تُحفظ في ملف Excel الفعلي. |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect/)() | يحمي ورقة العمل. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange/)(int, int, int, int) | يجعل نطاقًا من الخلايا للقراءة فقط. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells أولاً اجعل جميع الخلايا قابلة للتحرير عن طريق استدعاء طريقة SetAllCellsEditable. ثم استدعِ هذه الطريقة لتحديد نطاق الخلايا التي يجب أن تكون للقراءة فقط. |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption/)(int, string) | يضبط التسمية للصف. |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip/)(int, string) | يضبط نص تلميح رأس الصف. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly/)(int, bool) | يضبط صفًا للقراءة فقط بحيث لا يستطيع المستخدم حذفه من جانب العميل. هذه طريقة موسعة من GridWeb تحديدًا، لن تُحفظ ولن تؤثر في ملف Excel الفعلي. |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes/)() | يفك تجميد الألواح في ورقة العمل. |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows/)(int, int) | يفك تجميع الصفوف. |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect/)() | يلغي حماية الورقة. |

## الأحداث

| الاسم | الوصف |
| --- | --- |
| event [InitializeNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/initializenewbindrow/) | يحدث عندما تقوم الورقة بإنشاء صف ربط جديد وتحتاج إلى تهيئته. |

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


