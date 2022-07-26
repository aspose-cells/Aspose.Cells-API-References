---
title: PivotTable
second_title: Aspose.Cells لمرجع .NET API
description: وصف ملخص ل PivotTable .
type: docs
weight: 4690
url: /ar/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

وصف ملخص ل PivotTable .

```csharp
public class PivotTable : IDisposable
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription) { get; set; } | الحصول على وصف النص البديل |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle) { get; set; } | يحصل على عنوان النص البديل |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype) { get; set; } | الحصول على نوع التنسيق التلقائي لجدول PivotTable. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields) { get; } | إرجاع كائن PivotFields يتضمن كافة الحقول في تقرير PivotTable |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields) { get; } | إرجاع كائن PivotFields الذي يتم عرضه حاليًا كحقول أعمدة. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable يعرض الإجماليات الكلية للأعمدة. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption) { get; set; } | الحصول على التسمية التوضيحية لرأس العمود في PivotTable . |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange) { get; } | إرجاع كائن CellArea الذي يمثل range الذي يحتوي على منطقة العمود في تقرير PivotTable. للقراءة فقط. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort) { get; set; } | يشير إلى ما إذا كان يجب مراعاة القائمة المخصصة المضمنة عند فرز البيانات |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange) { get; } | إرجاع كائن CellArea الذي يمثل النطاق الذي يحتوي على منطقة البيانات في القائمة بين صف الرأس وصف الإدراج. للقراءة فقط. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield) { get; } | الحصول على كائن PivotField الذي يمثل جميع حقول البيانات في PivotTable. للقراءة فقط. سيكون الأمر init فقط عندما يكون هناك حقلين أو أكثر من حقول البيانات في DataPiovtFiels. يستخدم فقط لإضافة DataPivotField إلى صف / عمود PivotTable منطقة . الافتراضي في منطقة الصف. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields) { get; } | الحصول على كائن PivotField الذي يمثل جميع حقول البيانات في PivotTable. للقراءة فقط. سيكون الأمر init فقط عندما يكون هناك حقلين أو أكثر من حقول البيانات في DataPiovtFiels. يستخدم فقط لإضافة DataPivotField إلى صف / عمود PivotTable منطقة . الافتراضي في منطقة الصف. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource) { get; set; } | الحصول على مصدر بيانات الجدول المحوري وتعيينه. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة في الخلايا التي تحتوي على أخطاء. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems) { get; set; } | يشير إلى ما إذا كانت العناصر الموجودة في مناطق الصفوف والأعمدة مرئية عندما تكون منطقة البيانات في PivotTable فارغة. القيمة الافتراضية هي true . |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة في الخلايا التي تحتوي على قيم خالية. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting) { get; set; } | يحدد قيمة منطقية تشير إلى ما إذا كان المستخدم مسموحًا له بتحرير الخلايا في منطقة البيانات للمحور . تمكين تحرير الخلية في منطقة القيم |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown) { get; set; } | التعرف على ما إذا كان التنقل لأسفل ممكّنًا . |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog) { get; set; } | يشير إلى ما إذا كان مربع الحوار حقل PivotTable متوفرًا عندما ينقر المستخدم نقرًا مزدوجًا فوق حقل PivotTable . |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist) { get; set; } | الحصول على ما إذا كان يتم تمكين قائمة الحقول لجدول PivotTable. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard) { get; set; } | يشير إلى ما إذا كان معالج PivotTable متاحًا أم لا. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring) { get; set; } | الحصول على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء عندما تكون الخاصية DisplayErrorString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource) { get; } | يحصل على مصدر بيانات الاتصال الخارجي. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending) { get; set; } | تحدد قيمة منطقية تشير إلى ما إذا كانت الحقول في PivotTable يتم فرزها بترتيب غير افتراضي في قائمة الحقول. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname) { get; set; } | إرجاع تسمية السلسلة النصية المعروضة في عمود الإجمالي الكلي أو عنوان الصف . القيمة الافتراضية هي السلسلة "الإجمالي الكلي" . |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows) { get; set; } | يشير إلى ما إذا كان سيتم إضافة صفوف فارغة. تنطبق هذه الخاصية فقط على أنواع التنسيق التلقائي لـ PivotTable التي تحتاج إلى إضافة صفوف فارغة. |
| [Indent](../../aspose.cells.pivot/pivottable/indent) { get; set; } | يحدد زيادة المسافة البادئة للمحور المضغوط ويمكن استخدامه لتعيين تخطيط التقرير إلى نموذج مضغوط. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable قد تم تنسيقه تلقائيًا. خانة اختيار "جدول تنسيق تلقائي" الموجود في الخيار المحوري لـ Excel 2003 خانة الاختيار "احتواء عرض العمود تلقائيًا عند التحديث" الموجود في خيارات الجدول المحوري: تنسيق التخطيط لبرنامج Excel 2007 |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible) { get; set; } | يحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديث PivotTable ، إذا كان صحيحًا ، يجب أن تكون السلسلة أقل من أو تساوي 255 حرفًا ، لذلك إذا كانت السلسلة أكبر من 255 حرفًا ، فسيتم اقتطاعها . إذا كانت خاطئة ، فلن يكون للسلسلة القيود المذكورة أعلاه . القيمة الافتراضية هي صحيحة. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable يعرض التخطيط الكلاسيكي المحوري. (يتيح سحب الحقول في الشبكة) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters) { get; set; } | تحديد قيمة منطقية تشير إلى ما إذا كان يمكن تعيين عوامل تصفية متعددة على حقول PivotTable. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected) { get; set; } | يشير إلى ما إذا كان PivotTable محددًا أم لا. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles) { get; set; } | بت يحدد ما إذا كانت التسميات التوضيحية للعنصر المحوري على محور الصف تتكرر في كل صفحة مطبوعة للحقول المحورية في شكل جدول . |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable سيعاد حسابه فقط بناءً على طلب المستخدم. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels) { get; set; } | يشير إلى ما إذا كان عنصر الصف الخارجي ، وعنصر العمود ، والإجمالي الفرعي ، و والتسميات الإجمالية الكلية لتقرير PivotTable تستخدم خلايا مدمجة. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit) { get; set; } | تحديد قيمة منطقية تشير إلى ما إذا كان يمكن تعيين عوامل تصفية متعددة على حقول PivotTable. |
| [Name](../../aspose.cells.pivot/pivottable/name) { get; set; } | الحصول على اسم PivotTable |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring) { get; set; } | الحصول على السلسلة المعروضة في الخلايا التي تحتوي على قيم خالية عندما تكون الخاصية DisplayNullString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder) { get; set; } | الحصول على الترتيب الذي تتم به إضافة حقول الصفحة إلى تخطيط تقرير PivotTable. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields) { get; } | إرجاع كائن PivotFields الذي يتم عرضه حاليًا كحقول صفحة. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount) { get; set; } | الحصول على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters) { get; } | إرجاع كائن PivotFilterCollection . |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions) { get; } | الحصول على شروط التنسيق للجدول المحوري. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename) { get; set; } | الحصول على اسم النمط المحوري وتعيينه. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype) { get; set; } | الحصول على وتعيين نمط الجدول المحوري المضمن. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting) { get; set; } | يشير إلى ما إذا كان سيتم الاحتفاظ بالتنسيق عند تحديث PivotTable أو إعادة حسابه. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill) { get; set; } | يحدد قيمة منطقية تشير إلى ما إذا كان يجب طباعة مؤشرات الحفر. طباعة أزرار توسيع / طي عند عرضها على pivottable . |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles) { get; set; } | يشير إلى ما إذا تم تعيين عناوين الطباعة لورقة العمل على أساس في تقرير PivotTable. القيمة الافتراضية هي كاذبة. |
| [RefreshDataFlag](../../aspose.cells.pivot/pivottable/refreshdataflag) { get; set; } | يشير إلى ما إذا كان سيتم تحديث البيانات أم لا. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile) { get; set; } | يشير إلى ما إذا كان سيتم تحديث البيانات عند فتح الملف. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate) { get; } | الحصول على تاريخ آخر تحديث لـ PivotTable. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho) { get; } | الحصول على اسم المستخدم الذي قام آخر مرة بتحديث PivotTable |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields) { get; } | إرجاع كائن PivotFields الذي يتم عرضه حاليًا كحقول صف. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable يعرض الإجماليات الكلية للصفوف. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption) { get; set; } | الحصول على التسمية التوضيحية لرأس الصف في PivotTable . |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange) { get; } | إرجاع كائن CellArea الذي يمثل range الذي يحتوي على منطقة الصف في تقرير PivotTable. للقراءة فقط. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata) { get; set; } | يشير إلى ما إذا كان سيتم حفظ بيانات تقرير PivotTable مع المصنف. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips) { get; set; } | تحدد قيمة منطقية تشير إلى ما إذا كان يجب عرض تلميحات الأدوات لخلايا بيانات PivotTable. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill) { get; set; } | الحصول على ما إذا كانت أزرار التوسيع / الطي ستظهر أم لا. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol) { get; set; } | تحديد قيمة منطقية تشير إلى ما إذا كان سيتم تضمين أعمدة فارغة في الجدول |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow) { get; set; } | يحدد قيمة منطقية تشير إلى ما إذا كان سيتم تضمين صفوف فارغة في الجدول. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips) { get; set; } | يحدد قيمة منطقية تشير إلى ما إذا كان يجب حذف معلومات خاصية العضو من تلميحات أدوات PivotTable. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader) { get; set; } | يشير إلى ما إذا كان يجب تطبيق النمط المطبق على رأس العمود في الجدول المحوري. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes) { get; set; } | يشير إلى ما إذا كان تنسيق شريط العمود مطبقًا . |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn) { get; set; } | يشير إلى ما إذا كان تنسيق شريط العمود مطبقًا . |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader) { get; set; } | يشير إلى ما إذا كان يجب تطبيق النمط المطبق على رأس الصف في الجدول المحوري. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes) { get; set; } | يشير إلى ما إذا كان يتم تطبيق تنسيق شريط الصف. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption) { get; set; } | يشير إلى ما إذا كان يتم عرض التسمية التوضيحية لرأس الصف في تقرير PivotTable يشير إلى ما إذا كان عرض تسميات توضيحية للحقل وقائمة التصفية المنسدلة أم لا |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow) { get; set; } | يحدد قيمة منطقية تشير إلى ما إذا كان سيتم إظهار صف القيم. إظهار القيم row |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems) { get; set; } | يشير إلى ما إذا كانت عناصر حقل الصفحة المخفية في تقرير PivotTable مضمنة في الإجماليات الفرعية للصفوف والأعمدة ، وإجماليات الحظر ، والإجماليات الكلية. القيمة الافتراضية هي False . |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1) { get; } | إرجاع كائن CellArea الذي يمثل النطاق الذي يحتوي على تقرير PivotTable بأكمله ، ولكنه لا يتضمن حقول الصفحة. للقراءة فقط. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2) { get; } | إرجاع كائن CellArea الذي يمثل النطاق الذي يحتوي على تقرير PivotTable بأكمله ، يتضمن حقول الصفحة. للقراءة فقط. |
| [Tag](../../aspose.cells.pivot/pivottable/tag) { get; set; } | الحصول على سلسلة محفوظة بتقرير PivotTable . |

## طُرق

| اسم | وصف |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield)(string, string) | يضيف حقلاً محسوبًا إلى الحقل المحوري واسحبه إلى منطقة البيانات. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield_1)(string, string, bool) | يضيف حقلاً محسوبًا إلى الحقل المحوري. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_1)(PivotFieldType, int) | يضيف الحقل إلى المنطقة المحددة . |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea)(PivotFieldType, PivotField) | يضيف الحقل إلى المنطقة المحددة . |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_2)(PivotFieldType, string) | يضيف الحقل إلى المنطقة المحددة . |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata)() | حساب البيانات المحورية للخلايا. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange)() | حساب نطاق المحور المحوري . |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource)(string[]) | تعيين بيانات مصدر pivottable . Sheet1! $ A $ 1: $ C $ 3 |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata)() | مسح بيانات وتنسيقات PivotTable |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle)(PivotTable) | نسخ نمط مسمى من جدول محوري آخر. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose)() | يؤدي مهام محددة بواسطة التطبيق مرتبطة بتحرير الموارد غير المُدارة أو تحريرها أو إعادة تعيينها. |
| [Fields](../../aspose.cells.pivot/pivottable/fields)(PivotFieldType) | يحصل على الحقول المحددة حسب نوع الحقل. |
| [Format](../../aspose.cells.pivot/pivottable/format)(int, int, Style) | تنسيق الخلية في المنطقة المحورية |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall)(Style) | تنسيق كل الخلايا في المنطقة المحورية |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow)(int, Style) | تنسيق بيانات الصف في المنطقة المحورية |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname)(string) | الحصول على كائن الخلية بواسطة DisplayName الخاص بـ PivotField |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren)() | الحصول على الجداول المحورية الفرعية التي تستخدم بيانات PivotTable هذه كمصدر بيانات. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks)() | احصل على قائمة فهرس صف الجدول المحوري لفواصل الصفحات الأفقية |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource)() | الحصول على بيانات مصدر pivottable . |
| [Move](../../aspose.cells.pivot/pivottable/move#move_1)(string) | نقل PivotTable إلى موقع مختلف في ورقة العمل. |
| [Move](../../aspose.cells.pivot/pivottable/move#move)(int, int) | نقل PivotTable إلى موقع مختلف في ورقة العمل. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata)() | تحديث بيانات المحورية والإعداد من مصدر البيانات. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_1)(PivotFieldType, int) | يزيل حقل من منطقة حقل محددة |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield)(PivotFieldType, PivotField) | إزالة الحقل من منطقة حقل معين |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_2)(PivotFieldType, string) | يزيل حقل من منطقة حقل محددة |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield_1)(int) | يعين مجموعة الحقول التلقائية بواسطة PivotTable . |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield)(PivotField) | يعين مجموعة الحقول التلقائية بواسطة PivotTable . |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_3)(int, DateTime, DateTime, ArrayList, int) | يعين مجموعة الحقول اليدوية بواسطة PivotTable. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_2)(int, double, double, ArrayList, double) | يعين مجموعة الحقول اليدوية بواسطة PivotTable. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_1)(PivotField, DateTime, DateTime, ArrayList, int) | يعين مجموعة الحقول اليدوية بواسطة PivotTable. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield)(PivotField, double, double, ArrayList, double) | يعين مجموعة الحقول اليدوية بواسطة PivotTable. |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup_1)(int) | يعين فك التجميع بواسطة PivotTable |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup)(PivotField) | يعين فك التجميع بواسطة PivotTable |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform)() | تخطيطات PivotTable في شكل مضغوط. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform)() | تخطيطات PivotTable في شكل مخطط تفصيلي. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform)() | تخطيطات PivotTable في شكل جدولي. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage)(PivotField) | إظهار كافة صفحات عامل تصفية التقرير وفقًا لـ PivotField ، يجب أن يكون PivotField موجودًا في PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex)(int) | إظهار كافة صفحات تصفية التقرير وفقًا لفهرس الموضع في PageFields |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname)(string) | إظهار كافة صفحات عامل تصفية التقرير وفقًا لاسم PivotField ، ويجب أن يكون PivotField موجودًا في PageFields. |

### أمثلة

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

// تغيير سمات PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

// إضافة PivotFilter
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

// إضافة PivotFormatCondition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

// قم بعملك

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'أضف PivotFilter
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'أضف PivotFormatCondition
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
