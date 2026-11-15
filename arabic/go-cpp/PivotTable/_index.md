---
title: "PivotTable فئة"
linktitle: "PivotTable"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "PivotTable فئة. يغلف الكائن الذي يمثل pivottable في Go."
type: docs
weight: 200
url: /ar/go-cpp/pivottable/
---

## PivotTable class

وصف ملخص لجدول PivotTable.

```go

type PivotTable struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [Dispose](./dispose/) | يؤدي مهامًا محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [GetPivotCache](./getpivotcache/) | يحصل على مصدر البيانات. |
| [IsExcel2003Compatible](./isexcel2003compatible/) | يحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديث PivotTable، إذا كان true، يجب أن يكون النص أقل من أو يساوي 255 حرفًا، لذا إذا كان النص أطول من 255 حرفًا، سيتم قطعه. إذا كان false، لن يخضع النص للقيود المذكورة أعلاه. القيمة الافتراضية هي true. |
| [SetIsExcel2003Compatible](./setisexcel2003compatible/) | يحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديث PivotTable، إذا كان true، يجب أن يكون النص أقل من أو يساوي 255 حرفًا، لذا إذا كان النص أطول من 255 حرفًا، سيتم قطعه. إذا كان false، لن يخضع النص للقيود المذكورة أعلاه. القيمة الافتراضية هي true. |
| [GetRefreshedByWho](./getrefreshedbywho/) | يحصل على اسم آخر مستخدم قام بتحديث هذا PivotTable |
| [GetRefreshDate](./getrefreshdate/) | يحصل على آخر تاريخ ووقت عندما تم تحديث الـPivotTable. |
| [GetPivotTableStyle](./getpivottablestyle/) | يحصل على إعدادات TableStyle لهذا pivot table. |
| [SetPivotTableStyle](./setpivottablestyle/) | يحصل على إعدادات TableStyle لهذا pivot table. |
| [GetPivotTableStyleName](./getpivottablestylename/) | يحصل أو يعيّن اسم النمط للـpivot table. |
| [SetPivotTableStyleName](./setpivottablestylename/) | يحصل أو يعيّن اسم النمط للـpivot table. |
| [GetPivotTableStyleType](./getpivottablestyletype/) | يحصل ويعيّن نمط الـpivot table المدمج. |
| [SetPivotTableStyleType](./setpivottablestyletype/) | يحصل ويعيّن نمط الـpivot table المدمج. |
| [CopyStyle](./copystyle/) | ينسخ النمط المسمى من pivot table آخر. |
| [ShowReportFilterPage](./showreportfilterpage/) | اعرض جميع صفحات مرشح التقرير وفقًا لـPivotField، يجب أن يكون الـPivotField موجودًا في PageFields. |
| [ShowReportFilterPageByName](./showreportfilterpagebyname/) | اعرض جميع صفحات مرشح التقرير وفقًا لاسم الـPivotField، يجب أن يكون الـPivotField موجودًا في PageFields. |
| [ShowReportFilterPageByIndex](./showreportfilterpagebyindex/) | اعرض جميع صفحات مرشح التقرير وفقًا لمؤشر الموقع في PageFields. |
| [RemoveField_PivotFieldType_String](./removefield_pivotfieldtype_string/) | يزيل حقلًا من منطقة الحقول المحددة. |
| [RemoveField_PivotFieldType_Int](./removefield_pivotfieldtype_int/) | يزيل حقلًا من منطقة الـpivot المحددة. |
| [RemoveField_PivotFieldType_PivotField](./removefield_pivotfieldtype_pivotfield/) | إزالة حقل من منطقة الحقول المحددة. |
| [AddFieldToArea_PivotFieldType_String](./addfieldtoarea_pivotfieldtype_string/) | يضيف الحقل إلى المنطقة المحددة. |
| [AddFieldToArea_PivotFieldType_Int](./addfieldtoarea_pivotfieldtype_int/) | يضيف الحقل إلى المنطقة المحددة. |
| [AddFieldToArea_PivotFieldType_PivotField](./addfieldtoarea_pivotfieldtype_pivotfield/) | يضيف الحقل إلى المنطقة المحددة. |
| [AddCalculatedField_String_String_Bool](./addcalculatedfield_string_string_bool/) | يضيف حقلًا محسوبًا إلى pivot field. |
| [AddCalculatedField_String_String](./addcalculatedfield_string_string/) | يضيف حقلًا محسوبًا إلى pivot field ويسحبه إلى منطقة البيانات. |
| [GetFields](./getfields/) | يحصل على قائمة pivot field المحددة حسب المنطقة. |
| [GetColumnFields](./getcolumnfields/) | يرجع كائن PivotFields يُظهر حاليًا كحقول عمود. |
| [GetRowFields](./getrowfields/) | يرجع كائن PivotFields يُظهر حاليًا كحقول صف. |
| [GetPageFields](./getpagefields/) | يرجع كائن PivotFields يُظهر حاليًا كحقول صفحة. |
| [GetDataFields](./getdatafields/) | يحصل على كائن PivotField يمثل جميع حقول البيانات في PivotTable. للقراءة فقط. يتم تهيئته فقط عندما يكون هناك حقلان بيانات أو أكثر في DataPiovtFiels. يُستخدم فقط لإضافة DataPivotField إلى منطقة الصف/العمود في PivotTable. الافتراضي هو في منطقة الصف. |
| [GetValuesField](./getvaluesfield/) | يحصل على كائن PivotField يمثل جميع حقول البيانات في PivotTable. للقراءة فقط. يتم إنشاؤه فقط عندما يكون هناك حقلان بيانات أو أكثر في منطقة البيانات. بشكل افتراضي يكون في منطقة الصف. يمكنك سحبه إلى منطقة الصف/العمود باستخدام طريقة PivotTable.AddFieldToArea(). |
| [GetBaseFields](./getbasefields/) | يرجع جميع حقول الـpivot الأساسية في PivotTable. |
| [GetPivotFilters](./getpivotfilters/) | يرجع جميع مرشحات حقول الـpivot في pivot table. |
| [GetButtonArea](./getbuttonarea/) | يحصل على المنطقة التي تحتوي على زر الحقل. |
| [GetTopRightArea](./gettoprightarea/) | يمثل المنطقة الفارغة في أعلى يمين PivotTable (أعلى يسار للأوراق RTL). |
| [GetFilterArea](./getfilterarea/) | يحصل على مساحة منطقة الفلتر. |
| [GetColumnRange](./getcolumnrange/) | إرجاع كائن CellArea يمثل النطاق الذي يحتوي على منطقة الأعمدة في تقرير PivotTable. للقراءة فقط. |
| [GetRowRange](./getrowrange/) | إرجاع كائن CellArea يمثل النطاق الذي يحتوي على منطقة الصفوف في تقرير PivotTable. للقراءة فقط. |
| [GetDataBodyRange](./getdatabodyrange/) | إرجاع كائن CellArea يمثل النطاق الذي يحتوي على منطقة البيانات في القائمة بين صف الرأس وصف الإدراج. للقراءة فقط. |
| [GetTableRange1](./gettablerange1/) | إرجاع كائن CellArea يمثل النطاق الذي يحتوي على تقرير PivotTable بالكامل، لكنه لا يتضمن حقول الصفحات. للقراءة فقط. |
| [GetTableRange2](./gettablerange2/) | إرجاع كائن CellArea يمثل النطاق الذي يحتوي على تقرير PivotTable بالكامل، ويتضمن حقول الصفحات. للقراءة فقط. |
| [MoveTo_Int_Int](./moveto_int_int/) | ينقل PivotTable إلى موقع مختلف في ورقة العمل. |
| [MoveTo_Int_Int_Int](./moveto_int_int_int/) | ينقل PivotTable إلى موقع مختلف في ورقة العمل. |
| [MoveTo_String](./moveto_string/) | ينقل PivotTable إلى موقع مختلف في ورقة العمل. |
| [IsGridDropZones](./isgriddropzones/) | يشير إلى ما إذا كان تقرير PivotTable يعرض تخطيط PivotTable الكلاسيكي. (يتيح سحب الحقول في الشبكة) |
| [SetIsGridDropZones](./setisgriddropzones/) | يشير إلى ما إذا كان تقرير PivotTable يعرض تخطيط PivotTable الكلاسيكي. (يتيح سحب الحقول في الشبكة) |
| [GetShowColumnGrandTotals](./getshowcolumngrandtotals/) | يشير إلى ما إذا كان يجب عرض الإجماليات العامة للأعمدة في هذا PivotTable. |
| [SetShowColumnGrandTotals](./setshowcolumngrandtotals/) | يشير إلى ما إذا كان يجب عرض الإجماليات العامة للأعمدة في هذا PivotTable. |
| [GetShowRowGrandTotals](./getshowrowgrandtotals/) | يشير إلى ما إذا كان يجب عرض الإجماليات العامة للصفوف في PivotTable. |
| [SetShowRowGrandTotals](./setshowrowgrandtotals/) | يشير إلى ما إذا كان يجب عرض الإجماليات العامة للصفوف في PivotTable. |
| [GetDisplayNullString](./getdisplaynullstring/) | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة إذا كانت القيمة فارغة. |
| [SetDisplayNullString](./setdisplaynullstring/) | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة إذا كانت القيمة فارغة. |
| [GetNullString](./getnullstring/) | يحصل على السلسلة المعروضة في الخلايا التي تحتوي على قيم فارغة عندما تكون خاصية DisplayNullString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [SetNullString](./setnullstring/) | يحصل على السلسلة المعروضة في الخلايا التي تحتوي على قيم فارغة عندما تكون خاصية DisplayNullString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [GetDisplayErrorString](./getdisplayerrorstring/) | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة في الخلايا التي تحتوي على أخطاء. |
| [SetDisplayErrorString](./setdisplayerrorstring/) | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة في الخلايا التي تحتوي على أخطاء. |
| [GetDataFieldHeaderName](./getdatafieldheadername/) | يحصل على ويضبط اسم عنوان حقل منطقة القيمة في PivotTable. |
| [SetDataFieldHeaderName](./setdatafieldheadername/) | يحصل على ويضبط اسم عنوان حقل منطقة القيمة في PivotTable. |
| [GetErrorString](./geterrorstring/) | يحصل على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء عندما تكون خاصية DisplayErrorString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [SetErrorString](./seterrorstring/) | يحصل على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء عندما تكون خاصية DisplayErrorString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [IsAutoFormat](./isautoformat/) | يشير إلى ما إذا كان تقرير PivotTable يتم تنسيقه تلقائيًا. مربع الاختيار \"autoformat table\" الموجود في خيار PivotTable لبرنامج Excel 2003. |
| [SetIsAutoFormat](./setisautoformat/) | يشير إلى ما إذا كان تقرير PivotTable يتم تنسيقه تلقائيًا. مربع الاختيار \"autoformat table\" الموجود في خيار PivotTable لبرنامج Excel 2003. |
| [GetAutofitColumnWidthOnUpdate](./getautofitcolumnwidthonupdate/) | يشير إلى ما إذا كان يجب ضبط عرض العمود تلقائيًا عند التحديث. |
| [SetAutofitColumnWidthOnUpdate](./setautofitcolumnwidthonupdate/) | يشير إلى ما إذا كان يجب ضبط عرض العمود تلقائيًا عند التحديث. |
| [GetAutoFormatType](./getautoformattype/) | يحصل على ويضبط نوع التنسيق التلقائي لـ PivotTable. |
| [SetAutoFormatType](./setautoformattype/) | يحصل على ويضبط نوع التنسيق التلقائي لـ PivotTable. |
| [GetMergeLabels](./getmergelabels/) | يشير إلى ما إذا كان يجب دمج عناوين الصف أو العمود التي تمتد عبر عدة خلايا في خلية واحدة. |
| [SetMergeLabels](./setmergelabels/) | يشير إلى ما إذا كان يجب دمج عناوين الصف أو العمود التي تمتد عبر عدة خلايا في خلية واحدة. |
| [GetPreserveCellFormattingOnUpdate](./getpreservecellformattingonupdate/) | يشير إلى ما إذا كان يجب الحفاظ على تنسيق الخلية (PivotTableFormat) عند تحديث أو إعادة حساب PivotTable. |
| [SetPreserveCellFormattingOnUpdate](./setpreservecellformattingonupdate/) | يشير إلى ما إذا كان يجب الحفاظ على تنسيق الخلية (PivotTableFormat) عند تحديث أو إعادة حساب PivotTable. |
| [GetShowDrill](./getshowdrill/) | يحصل على ويضبط ما إذا كان يتم عرض أزرار التوسيع/الطي. |
| [SetShowDrill](./setshowdrill/) | يحصل على ويضبط ما إذا كان يتم عرض أزرار التوسيع/الطي. |
| [GetEnableDrilldown](./getenabledrilldown/) | يشير إلى ما إذا كان التفصيل (drilldown) مفعلاً. |
| [SetEnableDrilldown](./setenabledrilldown/) | يشير إلى ما إذا كان التفصيل (drilldown) مفعلاً. |
| [GetEnableFieldDialog](./getenablefielddialog/) | يشير إلى ما إذا كان مربع حوار حقل PivotTable متاحًا عندما ينقر المستخدم مزدوجًا على حقل PivotTable. |
| [SetEnableFieldDialog](./setenablefielddialog/) | يشير إلى ما إذا كان مربع حوار حقل PivotTable متاحًا عندما ينقر المستخدم مزدوجًا على حقل PivotTable. |
| [GetEnableFieldList](./getenablefieldlist/) | يشير إلى ما إذا كانت قائمة الحقول لـ PivotTable متاحة في عرض Excel. |
| [SetEnableFieldList](./setenablefieldlist/) | يشير إلى ما إذا كانت قائمة الحقول لـ PivotTable متاحة في عرض Excel. |
| [GetEnableWizard](./getenablewizard/) | يشير إلى ما إذا كان معالج PivotTable متاحًا. |
| [SetEnableWizard](./setenablewizard/) | يشير إلى ما إذا كان معالج PivotTable متاحًا. |
| [GetSubtotalHiddenPageItems](./getsubtotalhiddenpageitems/) | يشير إلى ما إذا كانت عناصر حقل الصفحة المخفية في تقرير PivotTable مشمولة في المجاميع الفرعية للصفوف والأعمدة، ومجاميع الكتل، والإجماليات العامة. القيمة الافتراضية هي False. |
| [SetSubtotalHiddenPageItems](./setsubtotalhiddenpageitems/) | يشير إلى ما إذا كانت عناصر حقل الصفحة المخفية في تقرير PivotTable مشمولة في المجاميع الفرعية للصفوف والأعمدة، ومجاميع الكتل، والإجماليات العامة. القيمة الافتراضية هي False. |
| [GetGrandTotalName](./getgrandtotalname/) | يعيد التسمية التي تُعرض في عنوان عمود أو صف الإجمالي الكلي. القيمة الافتراضية هي السلسلة "Grand Total". |
| [SetGrandTotalName](./setgrandtotalname/) | يعيد التسمية التي تُعرض في عنوان عمود أو صف الإجمالي الكلي. القيمة الافتراضية هي السلسلة "Grand Total". |
| [GetManualUpdate](./getmanualupdate/) | يحدد ما إذا كان تقرير PivotTable يُعاد حسابه فقط عند طلب المستخدم. |
| [SetManualUpdate](./setmanualupdate/) | يحدد ما إذا كان تقرير PivotTable يُعاد حسابه فقط عند طلب المستخدم. |
| [GetAllowMultipleFiltersPerField](./getallowmultiplefiltersperfield/) | يحدد قيمة منطقية تشير إلى ما إذا كان يمكن تعيين مرشحات متعددة على حقول PivotTable. |
| [SetAllowMultipleFiltersPerField](./setallowmultiplefiltersperfield/) | يحدد قيمة منطقية تشير إلى ما إذا كان يمكن تعيين مرشحات متعددة على حقول PivotTable. |
| [GetEnableDataValueEditing](./getenabledatavalueediting/) | يحدد قيمة منطقية تشير إلى ما إذا كان يُسمح للمستخدم بتحرير الخلايا في منطقة البيانات من PivotTable. تمكين تحرير الخلايا في منطقة القيم. |
| [SetEnableDataValueEditing](./setenabledatavalueediting/) | يحدد قيمة منطقية تشير إلى ما إذا كان يُسمح للمستخدم بتحرير الخلايا في منطقة البيانات من PivotTable. تمكين تحرير الخلايا في منطقة القيم. |
| [GetShowDataTips](./getshowdatatips/) | يحدد ما إذا كان يجب عرض تلميحات الأدوات لخلايا بيانات PivotTable. |
| [SetShowDataTips](./setshowdatatips/) | يحدد ما إذا كان يجب عرض تلميحات الأدوات لخلايا بيانات PivotTable. |
| [GetShowMemberPropertyTips](./getshowmemberpropertytips/) | يحدد قيمة منطقية تشير إلى ما إذا كان يجب حذف معلومات خصائص العضو من تلميحات أدوات PivotTable. |
| [SetShowMemberPropertyTips](./setshowmemberpropertytips/) | يحدد قيمة منطقية تشير إلى ما إذا كان يجب حذف معلومات خصائص العضو من تلميحات أدوات PivotTable. |
| [GetShowValuesRow](./getshowvaluesrow/) | يحدد ما إذا كان يتم إظهار صف القيم. |
| [SetShowValuesRow](./setshowvaluesrow/) | يحدد ما إذا كان يتم إظهار صف القيم. |
| [GetShowEmptyCol](./getshowemptycol/) | يحدد ما إذا كان يجب تضمين الأعمدة الفارغة في الجدول. |
| [SetShowEmptyCol](./setshowemptycol/) | يحدد ما إذا كان يجب تضمين الأعمدة الفارغة في الجدول. |
| [GetShowEmptyRow](./getshowemptyrow/) | يحدد ما إذا كان يجب تضمين الصفوف الفارغة في الجدول. |
| [SetShowEmptyRow](./setshowemptyrow/) | يحدد ما إذا كان يجب تضمين الصفوف الفارغة في الجدول. |
| [GetFieldListSortAscending](./getfieldlistsortascending/) | يحدد ما إذا كانت حقول PivotTable مرتبة بترتيب غير افتراضي في قائمة الحقول. |
| [SetFieldListSortAscending](./setfieldlistsortascending/) | يحدد ما إذا كانت حقول PivotTable مرتبة بترتيب غير افتراضي في قائمة الحقول. |
| [GetPrintDrill](./getprintdrill/) | يحدد قيمة منطقية تشير إلى ما إذا كان يجب طباعة مؤشرات الحفر. طباعة أزرار التوسيع/الطي عند عرضها على PivotTable. |
| [SetPrintDrill](./setprintdrill/) | يحدد قيمة منطقية تشير إلى ما إذا كان يجب طباعة مؤشرات الحفر. طباعة أزرار التوسيع/الطي عند عرضها على PivotTable. |
| [GetAltTextTitle](./getalttexttitle/) | يحصل على عنوان النص البديل ويضبطه. |
| [SetAltTextTitle](./setalttexttitle/) | يحصل على عنوان النص البديل ويضبطه. |
| [GetAltTextDescription](./getalttextdescription/) | يحصل على وصف النص البديل. |
| [SetAltTextDescription](./setalttextdescription/) | يحصل على وصف النص البديل. |
| [GetName](./getname/) | يحصل على اسم PivotTable. |
| [SetName](./setname/) | يحصل على اسم PivotTable. |
| [GetColumnHeaderCaption](./getcolumnheadercaption/) | يحصل على تسمية مخصصة لرأس العمود في PivotTable ويضبطها. |
| [SetColumnHeaderCaption](./setcolumnheadercaption/) | يحصل على تسمية مخصصة لرأس العمود في PivotTable ويضبطها. |
| [GetIndent](./getindent/) | يحدد مقدار الزيادة في المسافة البادئة للمحور المدمج ويمكن استخدامه لضبط تخطيط التقرير إلى الشكل المدمج. |
| [SetIndent](./setindent/) | يحدد مقدار الزيادة في المسافة البادئة للمحور المدمج ويمكن استخدامه لضبط تخطيط التقرير إلى الشكل المدمج. |
| [GetRowHeaderCaption](./getrowheadercaption/) | يحصل على تسمية مخصصة لرأس الصف في هذا PivotTable ويضبطها. |
| [SetRowHeaderCaption](./setrowheadercaption/) | يحصل على تسمية مخصصة لرأس الصف في هذا PivotTable ويضبطها. |
| [GetShowHeaders](./getshowheaders/) | ما إذا كان يجب إظهار تسميات حقول البيانات وتسمية حقول Pivot على محور الصف ومحور العمود في عرض PivotTable. |
| [SetShowHeaders](./setshowheaders/) | ما إذا كان يجب إظهار تسميات حقول البيانات وتسمية حقول Pivot على محور الصف ومحور العمود في عرض PivotTable. |
| [GetCustomListSort](./getcustomlistsort/) | يحدد ما إذا كان يجب أخذ القائمة المخصصة المدمجة في الاعتبار عند فرز البيانات. |
| [SetCustomListSort](./setcustomlistsort/) | يحدد ما إذا كان يجب أخذ القائمة المخصصة المدمجة في الاعتبار عند فرز البيانات. |
| [GetConditionalFormats](./getconditionalformats/) | يحصل على التنسيقات الشرطية لجدول Pivot. |
| [GetPageFieldOrder](./getpagefieldorder/) | يحصل على ترتيب إضافة حقول الصفحة إلى تخطيط تقرير PivotTable ويضبطه. |
| [SetPageFieldOrder](./setpagefieldorder/) | يحصل على ترتيب إضافة حقول الصفحة إلى تخطيط تقرير PivotTable ويضبطه. |
| [GetPageFieldWrapCount](./getpagefieldwrapcount/) | يحصل على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable. |
| [SetPageFieldWrapCount](./setpagefieldwrapcount/) | يحصل على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable. |
| [GetTag](./gettag/) | يحصل على سلسلة معرفة من قبل المستخدم وتضبطها والتي ترتبط بهذا العرض لPivotTable. |
| [SetTag](./settag/) | يحصل على سلسلة معرفة من قبل المستخدم وتضبطها والتي ترتبط بهذا العرض لPivotTable. |
| [GetSaveData](./getsavedata/) | يحدد ما إذا كان يتم حفظ بيانات تقرير PivotTable مع المصنف. |
| [SetSaveData](./setsavedata/) | يحدد ما إذا كان يتم حفظ بيانات تقرير PivotTable مع المصنف. |
| [GetRefreshDataOnOpeningFile](./getrefreshdataonopeningfile/) | يحدد ما إذا كان يتم تحديث البيانات عند فتح الملف. |
| [SetRefreshDataOnOpeningFile](./setrefreshdataonopeningfile/) | يحدد ما إذا كان يتم تحديث البيانات عند فتح الملف. |
| [GetSourceType](./getsourcetype/) | يحصل على نوع مصدر البيانات لجدول محوري. |
| [GetSourceDataConnections](./getsourcedataconnections/) | يحصل على مصادر بيانات الاتصال الخارجي. |
| [GetNamesOfSourceDataConnections](./getnamesofsourcedataconnections/) | يحصل على أسماء اتصالات مصدر البيانات الخارجي. |
| [GetDataSource](./getdatasource/) | يحصل ويضبط مصدر البيانات لجدول محوري. |
| [SetDataSource](./setdatasource/) | يحصل ويضبط مصدر البيانات لجدول محوري. |
| [ChangeDataSource](./changedatasource/) | غيّر مصدر البيانات لجدول محوري. |
| [GetSource](./getsource/) | احصل على مصدر البيانات لهذا جدول محوري. |
| [GetSource_Bool](./getsource_bool/) | احصل على مصدر البيانات لهذا جدول محوري. |
| [Refresh](./refresh/) | تحديث PivotCache من مصدر البيانات وحساب البيانات والنمط لعرض المحوري. |
| [CalculateData](./calculatedata/) | يحسب بيانات جدول محوري إلى الخلايا. |
| [CalculateData_PivotTableCalculateOption](./calculatedata_pivottablecalculateoption/) | يحسب جدول محوري مع الخيارات. |
| [GetPivotTablesWithSamePivotCache](./getpivottableswithsamepivotcache/) | يحصل على جميع جداول محورية ذات نفس PivotCache. |
| [ClearData](./cleardata/) | مسح البيانات وتنسيق عرض PivotTable. |
| [ClearFilters](./clearfilters/) | يمسح جميع الفلاتر لهذا جدول محوري. |
| [ClearAll](./clearall/) | إزالة جميع الحقول من المناطق. |
| [CalculateRange](./calculaterange/) | يحسب نطاق جدول محوري. |
| [FormatAll](./formatall/) | تنسيق جميع الخلايا في منطقة جدول محوري |
| [FormatRow](./formatrow/) | تنسيق بيانات الصف في منطقة جدول محوري |
| [Format_PivotArea_Style](./format_pivotarea_style/) | يقوم بتنسيق المنطقة المحددة من PivotTable. |
| [Format_CellArea_Style](./format_cellarea_style/) | يقوم بتنسيق المنطقة المحددة من PivotTable. |
| [Format_Int_Int_Style](./format_int_int_style/) | يقوم بتنسيق الخلية في منطقة جدول محوري |
| [SelectArea](./selectarea/) | حدد منطقة من عرض جدول محوري. |
| [ShowDetail](./showdetail/) | عرض تفاصيل عنصر واحد في منطقة البيانات إلى جدول جديد. |
| [GetPivotFormats](./getpivotformats/) | يحصل على جميع التنسيقات المطبقة على PivotTable. |
| [GetRepeatItemsOnEachPrintedPage](./getrepeatitemsoneachprintedpage/) | يشير إلى ما إذا كانت تسميات عنصر المحوري في منطقة الصف تتكرر في كل صفحة مطبوعة لحقول المحوري في الشكل الجدولي. |
| [SetRepeatItemsOnEachPrintedPage](./setrepeatitemsoneachprintedpage/) | يشير إلى ما إذا كانت تسميات عنصر المحوري في منطقة الصف تتكرر في كل صفحة مطبوعة لحقول المحوري في الشكل الجدولي. |
| [GetPrintTitles](./getprinttitles/) | يشير إلى ما إذا كانت عناوين الطباعة للورقة مضبوطة بناءً على تقرير PivotTable. القيمة الافتراضية هي false. |
| [SetPrintTitles](./setprinttitles/) | يشير إلى ما إذا كانت عناوين الطباعة للورقة مضبوطة بناءً على تقرير PivotTable. القيمة الافتراضية هي false. |
| [GetDisplayImmediateItems](./getdisplayimmediateitems/) | يشير إلى ما إذا كانت العناصر في مناطق الصف والعمود مرئية عندما تكون منطقة البيانات في PivotTable فارغة. القيمة الافتراضية هي true. |
| [SetDisplayImmediateItems](./setdisplayimmediateitems/) | يشير إلى ما إذا كانت العناصر في مناطق الصف والعمود مرئية عندما تكون منطقة البيانات في PivotTable فارغة. القيمة الافتراضية هي true. |
| [IsSelected](./isselected/) | يشير إلى ما إذا كان هذا PivotTable محددًا. |
| [SetIsSelected](./setisselected/) | يشير إلى ما إذا كان هذا PivotTable محددًا. |
| [GetShowPivotStyleRowHeader](./getshowpivotstylerowheader/) | يشير إلى ما إذا كان يجب تطبيق النمط على رأس الصف في جدول المحور. |
| [SetShowPivotStyleRowHeader](./setshowpivotstylerowheader/) | يشير إلى ما إذا كان يجب تطبيق النمط على رأس الصف في جدول المحور. |
| [GetShowPivotStyleColumnHeader](./getshowpivotstylecolumnheader/) | يشير إلى ما إذا كان يجب تطبيق النمط على رأس العمود في جدول المحور. |
| [SetShowPivotStyleColumnHeader](./setshowpivotstylecolumnheader/) | يشير إلى ما إذا كان يجب تطبيق النمط على رأس العمود في جدول المحور. |
| [GetShowPivotStyleRowStripes](./getshowpivotstylerowstripes/) | يشير إلى ما إذا كان تنسيق الشرائط للصفوف مطبقًا. |
| [SetShowPivotStyleRowStripes](./setshowpivotstylerowstripes/) | يشير إلى ما إذا كان تنسيق الشرائط للصفوف مطبقًا. |
| [GetShowPivotStyleColumnStripes](./getshowpivotstylecolumnstripes/) | يشير إلى ما إذا كان تنسيق الشرائط مطبقًا للعمود. |
| [SetShowPivotStyleColumnStripes](./setshowpivotstylecolumnstripes/) | يشير إلى ما إذا كان تنسيق الشرائط مطبقًا للعمود. |
| [GetShowPivotStyleLastColumn](./getshowpivotstylelastcolumn/) | يشير إلى ما إذا كان تنسيق العمود مطبقًا. |
| [SetShowPivotStyleLastColumn](./setshowpivotstylelastcolumn/) | يشير إلى ما إذا كان تنسيق العمود مطبقًا. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | يحصل على فواصل الصفحات الأفقية لهذا جدول المحور. |
| [ShowInCompactForm](./showincompactform/) | يُنسق عرض جدول المحور في الشكل المدمج. |
| [ShowInOutlineForm](./showinoutlineform/) | يُنسق جدول المحور في الشكل المخطط. |
| [ShowInTabularForm](./showintabularform/) | يُنسق جدول المحور في الشكل الجدولي. |
| [GetCellByDisplayName](./getcellbydisplayname/) | يحصل على كائن الخلية بواسطة الاسم المعروض لحقل المحور. |
| [GetDependentPivotTables](./getdependentpivottables/) | يحصل على جميع جداول المحور التي تستخدم هذا الجدول كمصدر بيانات لها. |
| [ExportViewToJson](./exportviewtojson/) | يصدّر عرض المحور كملف JSON. |
