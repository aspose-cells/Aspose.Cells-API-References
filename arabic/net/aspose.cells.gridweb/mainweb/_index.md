---
title: "الفئة MainWeb"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.MainWeb. الفئة الأصلية لعنصر تحكم GridWeb. للاستخدام الداخلي فقط"
type: docs
url: /ar/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

الفئة الأصلية لعنصر التحكم GridWeb. للاستخدام الداخلي فقط.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [MainWeb](mainweb/)() | البناء الافتراضي لعنصر تحكم MainWeb. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell/) { get; set; } | يحصل أو يضبط الخلية النشطة في الورقة الحالية. تم تغييرها لتصبح قابلة للكتابة منذ الإصدار 1.9.0.1. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor/) { get; set; } | يحدد لون خلفية الخلية النشطة. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor/) { get; set; } | يحدد لون الخلية النشطة. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor/) { get; set; } | يحدد لون خلفية رأس الصف/العمود النشط. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor/) { get; set; } | يحدد لون رأس الصف/العمود النشط. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet/) { get; } | يحصل على الورقة النشطة |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex/) { get; set; } | يحصل أو يضبط فهرس الورقة النشطة. يساوي WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle/) { get; set; } | يحدد نمط التبويب النشط. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath/) { get; set; } | يحصل أو يضبط مسار الويب لملفات السكريبت/الصورة للعنصر. على سبيل المثال: \"http://localhost/acw_client\". يمكنك أيضًا تعيين هذه القيمة في ملف web.config. أضف هذا القسم إلى قسم `<configuration>`:`<appSettings>``<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />``</appSettings>` |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl/) { get; set; } | يحصل أو يضبط عنوان URL للغة لملف العنصر. على سبيل المثال: \"/acw_client/lang_en.js\". بشكل افتراضي، يتم استخدام ملف إنجليزي مدمج. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart/) { get; set; } | يحصل أو يضبط ما إذا كانت صورة المخطط تُحدَّث أثناء تحديث قيمة الخلية. القيمة الافتراضية هي true. |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle/) { get; set; } | يحصل أو يضبط نمط الشريط السفلي للعنصر. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex/) { get; set; } | يحصل أو يضبط فهرس الصفحة الحالي في وضع الصفحات. |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine/) { get; set; } | يمثل محرك الحساب المخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons/) { get; } | يحصل على مجموعة أزرار الأوامر المخصصة |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename/) { get; set; } | يحصل أو يضبط اسم ملف النمط المخصص. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname/) { get; set; } | يحصل أو يضبط اسم الخط الافتراضي للعنصر. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize/) { get; set; } | يحصل أو يضبط حجم الخط الافتراضي للعنصر. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor/) { get; set; } | يحصل أو يضبط لون خط الشبكة الافتراضي. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم إظهار التلميحات. القيمة الافتراضية هي true. |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode/) { get; set; } | يحصل أو يضبط وضع التحرير للعنصر. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم استخدام استدعاء AJAX. القيمة الافتراضية هي true. |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تحميل بيانات الخلايا بطريقة غير متزامنة، يُنصح بتطبيق ذلك على ورقة واحدة تحتوي على أكثر من 10000 خلية. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تمكين عمليات الأعمدة من جانب العميل. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تمكين عمليات التجميد من جانب العميل. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تمكين عمليات الدمج من جانب العميل. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تمكين تغيير حجم الأعمدة والصفوف من جانب العميل. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تمكين عمليات الصفوف من جانب العميل. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تمكين حدث النقر المزدوج من جانب العميل. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تطبيق تأثير الضوء المعدني. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تمكين وضع الصفحات للعنصر. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تمكين مربع حوار النمط من جانب العميل. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم تمكين الصفحات بعد تصفية البيانات، سيصبح ساريًا عندما تكون EnablePaging true. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم فرض التحقق من صحة جانب العميل. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle/) { get; set; } | يحصل أو يضبط نمط الإطار للعنصر. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation/) { get; set; } | يحصل أو يضبط ما إذا كان GridWeb سيقوم بعملية الحفظ الافتراضية، القيمة الافتراضية هي true. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight/) { get; set; } | يحصل أو يضبط ارتفاع (System.Web.UI.WebControl.Unit) شريط الرأس العلوي للعنصر. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle/) { get; set; } | يحصل أو يضبط نمط شريط الرأس. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle/) { get; set; } | يحصل أو يضبط نمط شريط الرأس للعنصر. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth/) { get; set; } | يحصل أو يعيّن عرض ( System.Web.UI.WebControl.Unit ) أو شريط الرأس الأيسر للعنصر. |
| override [Height](../../aspose.cells.gridweb/mainweb/height/) { get; set; } | يحصل أو يعيّن ارتفاع ( System.Web.UI.WebControl.Unit ) للعنصر. |
| [IgnoreStyleWithNoData](../../aspose.cells.gridweb/mainweb/ignorestylewithnodata/) { get; set; } | يحصل أو يعيّن ما إذا كان GridWeb يتجاهل إظهار الصفوف أو الأعمدة التي لا تحتوي على قيم خلايا ولكنها لا تزال مُنسقة. إذا تم تعيينه إلى true، ستكون الأداء أفضل. القيمة الافتراضية هي false، مما يعني أنه إذا كان الصف/العمود المتتالي الأخير لا يحتوي على قيم خلايا ولكنه مُنسق، فسنظل نعرضه. هذا الخيار صالح فقط عندما يكون EnableAsync مساويًا لـ false. هذا الخيار لا يؤثر عندما يكون EnableAsync مساويًا لـ true، مما يعني أن GridWeb سيعرض جميع الصفوف/الأعمدة مع التنسيق. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula/) { get; set; } | يحصل أو يعيّن ما إذا كان سيتم حساب الصيغة بعد تغيّر قيمة الخلية أو بعد استيراد الملف. القيمة الافتراضية هي true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback/) { get; } | يحصل على قيمة تشير إلى ما إذا كان gridweb يتم تحميله استجابةً لإعادة إرسال العميل، أو إذا كان يتم تحميله والوصول إليه للمرة الأولى. |
| [LoadOptions](../../aspose.cells.gridweb/mainweb/loadoptions/) { get; set; } | يمثل خيارات التحميل لـ GridWeb. |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn/) { get; set; } | يحصل أو يعيّن الحد الأقصى لمؤشر العمود المعروض (مبني على الصفر) لورقة الويب. يستخدم العنصر القيمة الأكبر بين MaxColumn والعمود الأقصى لبيانات الورقة. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow/) { get; set; } | يحصل أو يعيّن الحد الأقصى لمؤشر الصف المعروض (مبني على الصفر) لورقة الويب. يستخدم العنصر القيمة الأكبر بين MaxRow والصف الأقصى لبيانات الورقة. |
| [Message](../../aspose.cells.gridweb/mainweb/message/) { get; set; } | يحصل أو يعيّن الرسالة الخاصة بالشبكة. |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn/) { get; set; } | يحصل أو يعيّن الحد الأدنى لمؤشر العمود المعروض (مبني على الصفر) لورقة الويب. يستخدم العنصر القيمة الأصغر بين MinColumn والعمود الأدنى لبيانات الورقة. |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow/) { get; set; } | يحصل أو يعيّن الحد الأدنى لمؤشر الصف المعروض (مبني على الصفر) لورقة الويب. يستخدم العنصر القيمة الأصغر بين MinRow والصف الأدنى لبيانات الورقة. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells/) { get; } | يحصل على مجموعة الخلايا التي تم تعديلها بواسطة العميل. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows/) { get; set; } | يحصل أو يعيّن ما إذا كان سيتم إظهار grouprows. |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان شريط التمرير الأفقي مخفيًا. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll/) { get; set; } | يحصل أو يعيّن ما إذا كان سيتم إظهار شريط التمرير. |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان شريط التمرير العمودي مخفيًا. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction/) { get; set; } | يحصل أو يعيّن اسم الدالة الجانبية للعميل التي يتم استدعاؤها عند انتهاء ajaxcall. يجب إعلان دالة العميل هكذا: `function GridAjaxcallFinished() { alert(this.id+" ajaxcall finished "); }` ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر الشبكة الذي يطلق الحدث. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction/) { get; set; } | يحصل أو يعيّن اسم الدالة الجانبية للعميل التي يتم استدعاؤها عندما تفشل عملية التحقق من صحة الخلية. يجب إعلان دالة العميل هكذا: `function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); }` ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر الشبكة الذي يطلق الحدث. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction/) { get; set; } | يحصل أو يعيّن الدالة الجانبية للعميل التي يتم استدعاؤها عند تحديد خلية. يجب إعلان دالة العميل هكذا: `function MyOnSelectCellAjaxCallBack(cell,customerdata) { }` ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر الشبكة الذي يطلق الحدث. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction/) { get; set; } | يحصل أو يعيّن الدالة الجانبية للعميل التي يتم استدعاؤها عند تحديد خلية. يجب إعلان دالة العميل هكذا: `function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, "test"); }` ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر الشبكة الذي يطلق الحدث. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/) { get; set; } | يحصل أو يعيّن الدالة الجانبية للعميل التي يتم استدعاؤها عند إلغاء تحديد خلية. يجب إعلان دالة العميل هكذا: `function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, "test"); }` ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر الشبكة الذي يطلق الحدث. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/) { get; set; } | يحصل أو يعيّن اسم الدالة الجانبية للعميل التي يتم استدعاؤها عند تحديث قيمة الخلية. يجب إعلان دالة العميل هكذا: `function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); }` ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر الشبكة الذي يطلق الحدث. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/) { get; set; } | الحصول أو تعيين الدالة الجانبية للعميل التي سيتم استدعاؤها عندما يتم عرض قائمة السياق. يجب إعلان دالة العميل كما يلي: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/) { get; set; } | الحصول أو تعيين الدالة الجانبية للعميل التي سيتم استدعاؤها عند النقر المزدوج على خلية. يجب إعلان دالة العميل كما يلي: function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, "test"); }ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction/) { get; set; } | الحصول أو تعيين الدالة الجانبية للعميل التي سيتم استدعاؤها عند النقر المزدوج على صف. يجب إعلان دالة العميل كما يلي: function MyOnRowDoubleClick(row) { alert(row); }ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction/) { get; set; } | الحصول أو تعيين اسم الدالة الجانبية للعميل التي سيتم استدعاؤها عند تهيئة الشبكة. يجب إعلان دالة العميل كما يلي: function MyOnGridInit(grid) { alert("The grid is initialized: " + grid.id); }ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto/) { get; set; } | الحصول أو تعيين ما إذا كان يجب ملاءمة الصفوف التي لا يكون ارتفاعها مخصصًا فقط، القيمة الافتراضية هي false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction/) { get; set; } | الحصول أو تعيين الدالة الجانبية للعميل التي سيتم استدعاؤها بعد تغيير فهرس الصفحة. تُطبق فقط عندما يكون EnablePaging صحيحًا. يجب إعلان دالة العميل كما يلي: function MyOnPageChange(index) { console.log("current page is:"+index); }ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction/) { get; set; } | الحصول أو تعيين الدالة الجانبية للعميل التي سيتم استدعاؤها قبل إرسال الصفحة من جانب العميل. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/) { get; set; } | الحصول أو تعيين الدالة الجانبية للعميل التي سيتم استدعاؤها عند تحديد شكل. يجب إعلان دالة العميل كما يلي: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction/) { get; set; } | الحصول أو تعيين الدالة الجانبية للعميل التي سيتم استدعاؤها قبل إرسال التحكم من جانب العميل. يجب إعلان دالة العميل كما يلي: function MyOnSubmit(arg, cancelEdit) { return true;} المتغيّر arg هو معطى الإرسال، يحتوي على الأمر الذي يُرسل إلى الخادم. المتغيّر cancelEdit هو قيمة منطقية تشير إلى ما إذا كان التحكم قد تجاهل إدخال المستخدم قبل الإرسال. سيستمر التحكم في الإرسال إذا أعادت الدالة true. ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize/) { get; set; } | الحصول أو تعيين حجم الصفحة في وضع الترقيم. |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle/) { get; set; } | الحصول أو تعيين النمط المسبق. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation/) { get; set; } | الحصول أو تعيين ما إذا كان يجب تحديث قيمة التحقق بعد تغيير قيمة الخلية. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow/) { get; set; } | الحصول أو تعيين ما إذا كان الصف المخفي يُعرض في GridControl، القيمة الافتراضية هي false. إذا كنت بحاجة إلى إظهار الصف المخفي لاحقًا، يجب تعيينه إلى true. |
| [RowHeightForCSV](../../aspose.cells.gridweb/mainweb/rowheightforcsv/) { get; set; } | الحصول أو تعيين قيمة ارتفاع الصف بالنقطة لملف csv، القيمة الافتراضية هي 14.5. |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor/) { get; set; } | يحدد لون زر السهم لشريط التمرير. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor/) { get; set; } | يحدد لون شريط التمرير للعنصر. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor/) { get; set; } | يحدد لون الخلفية للخلايا المحددة في نطاق الاختيار المتعدد. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor/) { get; set; } | يحدد لون الخلايا المحددة في نطاق الاختيار المتعدد. |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode/) { get; set; } | الحصول أو تعيين وضع الجلسة للشبكة. |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath/) { get; set; } | الحصول أو تعيين مسار تخزين ذاكرة التخزين المؤقت للجلسة عندما يكون وضع الجلسة File أو ViewState، إلخ: gridweb.SessionStorePath="c:/mytempdir/session"; ثم سيخزن بيانات الجلسة في c:/mytempdir/session |
| [Settings](../../aspose.cells.gridweb/mainweb/settings/) { get; set; } | يمثل إعدادات المصنف. |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton/) { get; set; } | الحصول أو تعيين ما إذا كان سيتم عرض زر إضافة ورقة العمل. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar/) { get; set; } | يحدد ما إذا كان سيتم عرض شريط الأوامر (يشمل شريط الأوامر وشريط التبويب) في أسفل العنصر. |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox/) { get; set; } | ما إذا كان Gridweb يعرض شريط أدوات صندوق التحرير كما في MS-EXCEL. إذا تم التفعيل، سيظهر صندوق تحرير للخلية الحالية في Gridweb. إذا فعلنا هذه الميزة، نحتاج إلى استيراد مكتبة jquery js في ملفات aspx الخاصة بك لدعم هذه الميزة الجديدة. جميع إصدارات jquery الحديثة مقبولة. إلخ. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop/) { get; set; } | يحدد ما إذا كان سيتم عرض شريط الأوامر (يتضمن شريط الأوامر وشريط الألسنة) في أعلى التحكم. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu/) { get; set; } | يحصل أو يحدد ما إذا كان سيتم عرض قائمة السياق. القيمة الافتراضية هي true. |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline/) { get; set; } | يحصل أو يحدد ما إذا كان سيتم عرض خطوط الشبكة الافتراضية للخلايا. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar/) { get; set; } | يحصل أو يحدد ما إذا كان سيتم عرض شريط الرأس |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading/) { get; set; } | يحدد ما إذا كان سيتم عرض مربع حوار التحميل أثناء الإرسال إلى الخادم. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition/) { get; set; } | يحدد الموضع الأيسر، العلوي (بالبيكسل) لعرض مربع حوار التحميل أثناء الإرسال إلى الخادم، إلخ. 100,200 يعني أن موضع مربع حوار التحميل الأيسر والعلوي هو 100px,200px. |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton/) { get; set; } | يحصل أو يحدد ما إذا كان سيتم عرض زر الحفظ. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton/) { get; set; } | يحصل أو يحدد ما إذا كان سيتم عرض زر الإرسال. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar/) { get; set; } | يحصل أو يحدد ما إذا كان سيتم عرض شريط الألسنة. |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation/) { get; set; } | يحصل أو يحدد ما إذا كان زر تنقل الألسنة معروضًا، القيمة الافتراضية هي true. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton/) { get; set; } | يحصل أو يحدد ما إذا كان سيتم عرض زر التراجع. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap/) { get; set; } | يحدد ما إذا كان سيتم لف المحتوى داخل نطاق الخلية. القيمة الافتراضية هي true. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle/) { get; set; } | يحصل أو يحدد نمط شريط الألسنة. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight/) { get; set; } | يحصل أو يحدد ما إذا كان GridWeb يستخدم ارتفاع صفحة العميل كارتفاع للتحكم، مناسب عندما يتم تعيين Height="100%"، القيمة الافتراضية هي false. |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft/) { get; set; } | يحصل أو يحدد موضع شريط التمرير في لوحة عرض الشبكة. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop/) { get; set; } | يحصل أو يحدد موضع شريط التمرير في لوحة عرض الشبكة. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle/) { get; set; } | يحصل أو يحدد نمط لوحة عرض البيانات. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets/) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width/) { get; set; } | يحصل أو يحدد عرض (System.Web.UI.WebControl.Unit) للتحكم. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets/) { get; } | يحصل أو يحدد مجموعة أوراق العمل. |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode/) { get; set; } | يحصل أو يحدد ما إذا كان سيتم استخدام نمط XHTML، القيمة الافتراضية هي true. |
| static [DPI](../../aspose.cells.gridweb/mainweb/dpi/) { get; set; } | يحصل / يحدد DPI للجهاز. |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath/) { get; set; } | يحصل أو يحدد مسار تخزين الصور لدفتر العمل، جميع الأشكال والصور سيتم تخزينها في هذا الدليل، المسار الافتراضي هو acwcache تحت دليل قاعدة التطبيق الحالي، يحتاج المستخدمون إلى تنفيذ خدمة جدولة لتنظيف الملفات التي انتهت مدة الجلسة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula/)() | يحسب نتيجة الصيغ. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind/)() | ربط التحكم وجميع عناصره الفرعية بمصدر البيانات الخاص به. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose/)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile)(Stream) | يستورد من تدفق ملف Excel، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_2)(string) | يستورد من ملف Excel. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_1)(Stream, string) | يستورد من تدفق ملف Excel، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_3)(string, string) | يستورد من ملف Excel. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile)(Stream) | يقوم بتحميل البيانات من تدفق ملف CSV. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile_1)(string) | يقوم بتحميل البيانات من ملف CSV. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile)(Stream) | يقوم بتحميل البيانات من تدفق ملف HTML. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile_1)(string) | يقوم بتحميل البيانات من ملف HTML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | يقوم بتحميل البيانات من تدفق ملف SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | يقوم بتحميل البيانات من ملف SpreadSheetML. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape/)() | تحديث جميع صور المخططات للورقة النشطة. |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag/)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile)(Stream) | يحفظ البيانات إلى تدفق ملف CSV. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile_1)(string) | يحفظ البيانات إلى ملف CSV. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile/)(string) | يحفظ بيانات النمط الحالية للتحكم في ملف XML. يمكن استخدامه لإنشاء ملف نمط مخصص. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile)(Stream) | يحفظ البيانات إلى تدفق ملف HTML. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile_1)(string) | يحفظ البيانات إلى ملف HTML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | يحفظ البيانات إلى تدفق ملف SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | يحفظ البيانات إلى ملف SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile)(Stream) | يحفظ أوراق العمل إلى ملف إكسل. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_3)(string) | يحفظ أوراق العمل إلى ملف إكسل بصيغة Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | يحفظ أوراق العمل إلى ملف إكسل. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_2)(Stream, GridSaveOptions) | يحفظ أوراق العمل إلى ملف إكسل. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_4)(string, GridSaveFormat) | يحفظ أوراق العمل إلى ملف إكسل. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_5)(string, GridSaveOptions) | يحفظ أوراق العمل إلى ملف إكسل. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle/)(Stream) | يحدد ملف النمط المخصص من تدفق يشمل تدفق ملف من القرص أو تدفق الذاكرة. |

## الأحداث

| الاسم | الوصف |
| --- | --- |
| event [AfterColumnFilter](../../aspose.cells.gridweb/mainweb/aftercolumnfilter/) | يحدث بعد تصفية العمود. |
| event [AjaxCallFinished](../../aspose.cells.gridweb/mainweb/ajaxcallfinished/) | يتم إطلاقه عندما ينتهي تحديث الـ ajax للعنصر. (يجب ضبط EnableAJAX على true) |
| event [BeforeColumnFilter](../../aspose.cells.gridweb/mainweb/beforecolumnfilter/) | يحدث قبل تصفية العمود. |
| event [CellClickOnAjax](../../aspose.cells.gridweb/mainweb/cellclickonajax/) | يحدث عندما يتم النقر على الخلية، ويحتاج إلى إجراء ajaxcallback لهذا الحدث. |
| event [CellClientUpdate](../../aspose.cells.gridweb/mainweb/cellclientupdate/) | يحدث عندما يحدث تحديث خلية من جانب العميل. عندما يتم إطلاق هذا الحدث، يحتوي المتغير e.Argument على اسم الأمر. |
| event [CellCommand](../../aspose.cells.gridweb/mainweb/cellcommand/) | يحدث عندما يتم النقر على ارتباط الأمر في الخلية. عندما يتم إطلاق هذا الحدث، يحتوي المتغير e.Argument على اسم الأمر. |
| event [CellDoubleClick](../../aspose.cells.gridweb/mainweb/celldoubleclick/) | يحدث عندما يتم النقر المزدوج على الخلية. |
| event [CellError](../../aspose.cells.gridweb/mainweb/cellerror/) | يحدث عندما يكون هناك خطأ في قيمة إدخال الخلية. |
| event [CellModifiedOnAjax](../../aspose.cells.gridweb/mainweb/cellmodifiedonajax/) | يحدث عندما يتم تعديل الخلية في ajaxcall. |
| event [ColumnDeleted](../../aspose.cells.gridweb/mainweb/columndeleted/) | يحدث عندما يقوم المستخدم بحذف عمود من القائمة الجانبية للعميل. |
| event [ColumnDeleting](../../aspose.cells.gridweb/mainweb/columndeleting/) | يحدث عندما يحاول المستخدم حذف عمود من القائمة الجانبية للعميل. يمكنك معالجة هذا الحدث وضبط المتغير cancel على True لإلغاء عملية الحذف. |
| event [ColumnDoubleClick](../../aspose.cells.gridweb/mainweb/columndoubleclick/) | يحدث عندما يتم النقر المزدوج على رأس العمود. |
| event [ColumnInserted](../../aspose.cells.gridweb/mainweb/columninserted/) | يحدث عندما يقوم المستخدم بإدراج عمود من القائمة الجانبية للعميل. |
| event [CustomCommand](../../aspose.cells.gridweb/mainweb/customcommand/) | يحدث عندما ينقر المستخدم على زر أمر مخصص. |
| event [LoadCustomData](../../aspose.cells.gridweb/mainweb/loadcustomdata/) | يتم إطلاقه عندما يتم ضبط SessionMode للعنصر على Custom ويحتاج إلى تحميل بيانات الورقة. يمكنك معالجة هذا الحدث في وضع Session مخصص لتحميل بيانات الورقة من ملف أو قاعدة بيانات. |
| event [PageIndexChanged](../../aspose.cells.gridweb/mainweb/pageindexchanged/) | يحدث عندما يتغير فهرس صفحة الورقة للعنصر. |
| event [RowDeleted](../../aspose.cells.gridweb/mainweb/rowdeleted/) | يحدث عندما يكون المستخدم قد حذف صفًا من القائمة الجانبية للعميل. |
| event [RowDeleting](../../aspose.cells.gridweb/mainweb/rowdeleting/) | يحدث عندما يحاول المستخدم حذف صف من القائمة الجانبية للعميل. يمكنك معالجة هذا الحدث وإلقاء استثناء RejectDeleteException لإلغاء عملية الحذف. |
| event [RowDoubleClick](../../aspose.cells.gridweb/mainweb/rowdoubleclick/) | يحدث عندما يتم النقر المزدوج على رأس الصف. |
| event [RowInserted](../../aspose.cells.gridweb/mainweb/rowinserted/) | يحدث عندما يقوم المستخدم بإدراج صف من القائمة الجانبية للعميل. |
| event [SaveCommand](../../aspose.cells.gridweb/mainweb/savecommand/) | يحدث عندما يتم النقر على زر "save". |
| event [SheetAdded](../../aspose.cells.gridweb/mainweb/sheetadded/) | يحدث عندما يضيف المستخدم ورقة عمل من قائمة شريط الأدوات. |
| event [SheetDataUpdated](../../aspose.cells.gridweb/mainweb/sheetdataupdated/) | يحدث عندما يكون العنصر قد حمّل البيانات المرسلة وقام بتحديث بيانات الورقة. |
| event [SheetTabClick](../../aspose.cells.gridweb/mainweb/sheettabclick/) | يحدث عندما يتم النقر على تبويب الورقة. |
| event [SubmitCommand](../../aspose.cells.gridweb/mainweb/submitcommand/) | يحدث عندما يتم النقر على زر "submit". |
| event [UndoCommand](../../aspose.cells.gridweb/mainweb/undocommand/) | يحدث عندما يتم النقر على زر "undo". |

### أمثلة

```csharp
[C#]
	GridWeb GridWeb1 = new GridWeb();
//قم بأعمالك
```

### انظر أيضًا

* class [ExtWebControl](../extwebcontrol/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


