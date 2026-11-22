---
title: "الفئة PivotTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Pivot.PivotTable. وصف ملخص لـ PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

وصف ملخص لجدول محوري.

```csharp
public class PivotTable : IDisposable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllowMultipleFiltersPerField](../../aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/) { get; set; } | يحدد قيمة منطقية تشير إلى ما إذا كانت حقول PivotTable يمكن أن تحتوي على فلاتر متعددة مضبوطة عليها. |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription/) { get; set; } | يحصل على وصف النص البديل. |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle/) { get; set; } | يحصل على عنوان النص البديل ويضبطه. |
| [AutofitColumnWidthOnUpdate](../../aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/) { get; set; } | يشير إلى ما إذا كان يجب ضبط عرض العمود تلقائيًا عند التحديث |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype/) { get; set; } | يحصل على نوع التنسيق التلقائي لـ PivotTable ويضبطه. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields/) { get; } | يرجع جميع حقول Pivot الأساسية في PivotTable. |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields/) { get; } | يرجع كائن PivotFields الذي يُظهر حاليًا كحقول عمود. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان تقرير PivotTable يعرض الإجماليات العامة للأعمدة. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption/) { get; set; } | يحصل على تسمية مخصصة لرأس العمود في PivotTable ويضبطها. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange/) { get; } | يرجع كائن CellArea الذي يمثل النطاق الذي يحتوي على منطقة العمود في تقرير PivotTable. للقراءة فقط. |
| [ConditionalFormats](../../aspose.cells.pivot/pivottable/conditionalformats/) { get; } | يحصل على التنسيقات الشرطية لجدول Pivot. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort/) { get; set; } | يشير إلى ما إذا كان يجب أخذ القائمة المخصصة المدمجة في الاعتبار عند فرز البيانات |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange/) { get; } | يرجع كائن [`CellArea`](../../aspose.cells/cellarea/) الذي يمثل النطاق الذي يحتوي على منطقة البيانات في القائمة بين صف الرأس وصف الإدراج. للقراءة فقط. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield/) { get; } | (**Obsolete.**) يحصل على كائن [`PivotField`](../pivotfield/) الذي يمثل جميع حقول البيانات في PivotTable. للقراءة فقط. يتم إنشاؤه فقط عندما يكون هناك حقلان أو أكثر من حقول البيانات في منطقة البيانات. بشكل افتراضي يكون في منطقة الصف. يمكنك سحبه إلى منطقة الصف/العمود باستخدام طريقة PivotTable.AddFieldToArea(). |
| [DataFieldHeaderName](../../aspose.cells.pivot/pivottable/datafieldheadername/) { get; set; } | يحصل على اسم رأس حقل منطقة القيمة في PivotTable ويضبطه. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields/) { get; } | يحصل على [`PivotFieldCollection`](../pivotfieldcollection/) الذي يمثل جميع حقول البيانات في PivotTable. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource/) { get; set; } | يحصل على مصدر البيانات لجدول Pivot ويضبطه. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring/) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة في الخلايا التي تحتوي على أخطاء. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems/) { get; set; } | يشير إلى ما إذا كانت العناصر في مناطق الصف والعمود مرئية عندما تكون منطقة البيانات في PivotTable فارغة. القيمة الافتراضية هي true. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring/) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة إذا كانت القيمة فارغة. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting/) { get; set; } | يحدد قيمة منطقية تشير إلى ما إذا كان يُسمح للمستخدم بتحرير الخلايا في منطقة البيانات من PivotTable. القيمة الافتراضية هي false. |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown/) { get; set; } | يشير إلى ما إذا كان التفصيل (drilldown) مفعلاً. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog/) { get; set; } | يشير إلى ما إذا كان مربع حوار PivotTable Field متاحًا عندما ينقر المستخدم مزدوجًا على حقل PivotTable. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist/) { get; set; } | يشير إلى ما إذا كانت قائمة الحقول لـ PivotTable متاحة في عرض Excel. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard/) { get; set; } | يشير إلى ما إذا كان معالج PivotTable متاحًا. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring/) { get; set; } | يحصل على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء عندما تكون خاصية DisplayErrorString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource/) { get; } | (**Obsolete.**) يحصل على مصدر بيانات الاتصال الخارجي. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending/) { get; set; } | يشير إلى ما إذا كانت الحقول في PivotTable مرتبة بترتيب غير افتراضي في قائمة الحقول. |
| [FilterArea](../../aspose.cells.pivot/pivottable/filterarea/) { get; } | يحصل على مساحة منطقة الفلتر. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname/) { get; set; } | يعيد التسمية التي تُعرض في عنوان عمود أو صف الإجمالي الكلي. القيمة الافتراضية هي السلسلة "Grand Total". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان يجب إضافة صفوف فارغة. هذه الخاصية تنطبق فقط على أنواع تنسيق PivotTable التلقائي التي تحتاج إلى إضافة صفوف فارغة. |
| [Indent](../../aspose.cells.pivot/pivottable/indent/) { get; set; } | يحدد زيادة المسافة البادئة للمحور المدمج ويمكن استخدامه لتعيين تخطيط التقرير إلى الشكل المدمج. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat/) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable مُنسقًا تلقائيًا. مربع الاختيار "autoformat table" الموجود في خيار PivotTable لبرنامج Excel 2003. |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible/) { get; set; } | يحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديث PivotTable، إذا كانت true، يجب أن تكون السلسلة أقل من أو تساوي 255 حرفًا، لذا إذا كانت السلسلة أطول من 255 حرفًا، سيتم قطعها. إذا كانت false، لن تخضع السلسلة للقيود المذكورة أعلاه. القيمة الافتراضية هي true. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones/) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable يعرض تخطيط PivotTable الكلاسيكي. (يمكّن سحب الحقول في الشبكة) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters/) { get; set; } | (**Obsolete.**) يحدد قيمة منطقية تشير إلى ما إذا كان يمكن للحقول في PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected/) { get; set; } | يشير إلى ما إذا كان PivotTable هذا محددًا. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان يجب تكرار أسماء PivotItem في أعلى كل صفحة مطبوعة. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate/) { get; set; } | يشير إلى ما إذا كان تقرير PivotTable يُعاد حسابه فقط عند طلب المستخدم. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels/) { get; set; } | يحصل أو يضبط ما إذا كان يجب دمج تسميات حقول الصف/العمود التي تمتد عبر خلايا متعددة. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit/) { get; set; } | (**Obsolete.**) يحدد قيمة منطقية تشير إلى ما إذا كان يمكن للحقول في PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها. |
| [Name](../../aspose.cells.pivot/pivottable/name/) { get; set; } | يحصل على اسم PivotTable |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring/) { get; set; } | يحصل على السلسلة المعروضة في الخلايا التي تحتوي على قيم فارغة عندما تكون خاصية DisplayNullString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder/) { get; set; } | يحصل ويضبط الترتيب الذي تُضاف به حقول الصفحة إلى تخطيط تقرير PivotTable. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields/) { get; } | يعيد مجموعة [`PivotFieldCollection`](../pivotfieldcollection/) التي تُظهر حاليًا كحقول صفحة. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount/) { get; set; } | يحصل على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable. |
| [PivotCache](../../aspose.cells.pivot/pivottable/pivotcache/) { get; } | يحصل على مصدر البيانات. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters/) { get; } | يعيد جميع الفلاتر في جدول PivotTable. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions/) { get; } | (**Obsolete.**) يحصل على شروط التنسيق لجدول المحور. |
| [PivotFormats](../../aspose.cells.pivot/pivottable/pivotformats/) { get; } | يحصل على جميع تنسيقات الخلايا المطبقة على جدول المحور هذا. |
| [PivotTableStyle](../../aspose.cells.pivot/pivottable/pivottablestyle/) { get; set; } | يحصل على إعدادات TableStyle لجدول المحور هذا. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename/) { get; set; } | يحصل أو يضبط اسم النمط لجدول المحور. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype/) { get; set; } | يحصل ويضبط نمط جدول المحور المدمج. |
| [PreserveCellFormattingOnUpdate](../../aspose.cells.pivot/pivottable/preservecellformattingonupdate/) { get; set; } | يشير إلى ما إذا كان يجب الحفاظ على تنسيق الخلية ([`PivotTableFormat`](../pivottableformat/)) عند تحديث أو إعادة حساب جدول المحور. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان تنسيق الخلية ([`PivotTableFormat`](../pivottableformat/)) محفوظًا عند تحديث أو إعادة حساب جدول المحور. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill/) { get; set; } | يحدد قيمة منطقية تشير إلى ما إذا كان يجب طباعة مؤشرات الحفر. طباعة أزرار التوسيع/الطي عند عرضها على جدول المحور. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles/) { get; set; } | يشير إلى ما إذا كانت عناوين الطباعة لورقة العمل مضبوطة بناءً على تقرير جدول المحور. القيمة الافتراضية هي false. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile/) { get; set; } | يشير إلى ما إذا كان يتم تحديث البيانات عند فتح الملف. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate/) { get; } | يحصل على تاريخ ووقت آخر مرة تم فيها تحديث جدول المحور. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho/) { get; } | يحصل على اسم آخر مستخدم قام بتحديث جدول المحور هذا |
| [RepeatItemsOnEachPrintedPage](../../aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/) { get; set; } | يشير إلى ما إذا كانت تسميات عنصر المحور في منطقة الصف تُكرر في كل صفحة مطبوعة لحقول المحور في الشكل الجدولي. |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields/) { get; } | يرجع مجموعة [`PivotFieldCollection`](../pivotfieldcollection/) التي تُعرض حاليًا كحقول صف. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان يجب إظهار الإجماليات العامة للصفوف في جدول المحور هذا. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption/) { get; set; } | يحصل ويضبط التسمية المخصصة لرأس الصف في جدول المحور هذا. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange/) { get; } | يرجع كائن CellArea الذي يمثل النطاق الذي يحتوي على منطقة الصف في تقرير جدول المحور. للقراءة فقط. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata/) { get; set; } | يشير إلى ما إذا كانت بيانات تقرير جدول المحور محفوظة مع المصنف. |
| [ShowColumnGrandTotals](../../aspose.cells.pivot/pivottable/showcolumngrandtotals/) { get; set; } | يشير إلى ما إذا كان يجب إظهار الإجماليات العامة للأعمدة في جدول المحور هذا. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips/) { get; set; } | يشير إلى ما إذا كان يجب عرض تلميحات الأدوات لخلايا بيانات جدول المحور. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill/) { get; set; } | يحصل ويضبط ما إذا كان يتم عرض أزرار التوسيع/الطي. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol/) { get; set; } | يشير إلى ما إذا كان يجب تضمين الأعمدة الفارغة في الجدول |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow/) { get; set; } | يشير إلى ما إذا كان يجب تضمين الصفوف الفارغة في الجدول. |
| [ShowHeaders](../../aspose.cells.pivot/pivottable/showheaders/) { get; set; } | ما إذا كان يجب إظهار تسميات حقول البيانات وتسميات حقول المحور على محور الصف ومحور العمود في عرض جدول المحور. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips/) { get; set; } | يحدد قيمة منطقية تشير إلى ما إذا كان يجب حذف معلومات خصائص العضو من تلميحات أدوات جدول المحور. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader/) { get; set; } | يشير إلى ما إذا كان يجب تطبيق النمط على عنوان العمود في جدول المحور. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/) { get; set; } | يشير إلى ما إذا تم تطبيق تنسيق الشرائط للعمود. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn/) { get; set; } | يشير إلى ما إذا تم تطبيق تنسيق العمود. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader/) { get; set; } | يشير إلى ما إذا كان يجب تطبيق النمط على عنوان الصف في جدول المحور. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes/) { get; set; } | يشير إلى ما إذا تم تطبيق تنسيق الشرائط للصف. |
| [ShowRowGrandTotals](../../aspose.cells.pivot/pivottable/showrowgrandtotals/) { get; set; } | يشير إلى ما إذا كان يجب إظهار الإجماليات العامة للصفوف في جدول المحور. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان عنوان رأس الصف معروضًا في تقرير PivotTable يشير إلى ما إذا كانت عناوين حقول العرض والقوائم المنسدلة للفلتر معروضة. |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow/) { get; set; } | يشير إلى ما إذا كان صف القيم معروضًا. |
| [SourceType](../../aspose.cells.pivot/pivottable/sourcetype/) { get; } | يحصل على نوع مصدر البيانات لجدول المحور. |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems/) { get; set; } | يشير إلى ما إذا كانت عناصر حقل الصفحة المخفية في تقرير PivotTable مشمولة في المجاميع الفرعية للصفوف والأعمدة، ومجاميع الكتل، والإجماليات العامة. القيمة الافتراضية هي False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1/) { get; } | يرجع كائن CellArea يمثل النطاق الذي يحتوي على تقرير PivotTable بالكامل، لكنه لا يتضمن حقول الصفحة. للقراءة فقط. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2/) { get; } | يرجع كائن CellArea يمثل النطاق الذي يحتوي على تقرير PivotTable بالكامل، ويتضمن حقول الصفحة. للقراءة فقط. |
| [Tag](../../aspose.cells.pivot/pivottable/tag/) { get; set; } | يحصل على ويضبط سلسلة معرفة من قبل المستخدم مرتبطة بهذا العرض لجدول PivotTable. |
| [TopRightArea](../../aspose.cells.pivot/pivottable/toprightarea/) { get; } | يمثل المنطقة الفارغة في أعلى يمين جدول PivotTable (أعلى يسار للأوراق RTL). |
| [ValuesField](../../aspose.cells.pivot/pivottable/valuesfield/) { get; } | يحصل على كائن [`PivotField`](../pivotfield/) يمثل جميع حقول البيانات في جدول PivotTable. للقراءة فقط. سيتم إنشاؤه فقط عندما يكون هناك حقلان بيانات أو أكثر في منطقة البيانات. بشكل افتراضي يكون في منطقة الصف. يمكنك سحبه إلى منطقة الصف/العمود باستخدام طريقة PivotTable.AddFieldToArea(). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield)(string, string) | يضيف حقلًا محسوبًا إلى حقل المحور ويسحبه إلى منطقة البيانات. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield_1)(string, string, bool) | يضيف حقلًا محسوبًا إلى حقل المحور. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_1)(PivotFieldType, int) | يضيف الحقل إلى المنطقة المحددة. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea)(PivotFieldType, PivotField) | يضيف الحقل إلى المنطقة المحددة. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_2)(PivotFieldType, string) | يضيف الحقل إلى المنطقة المحددة. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata_1)() | يحسب بيانات جدول المحور إلى الخلايا. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata)(PivotTableCalculateOption) | يحسب جدول المحور مع الخيارات. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange/)() | يحسب نطاق جدول المحور. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource/)(string[]) | غيّر مصدر البيانات لجدول المحور. |
| [ClearAll](../../aspose.cells.pivot/pivottable/clearall/)() | أزل جميع الحقول من المناطق. |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata/)() | امسح البيانات وتنسيق عرض PivotTable. |
| [ClearFilters](../../aspose.cells.pivot/pivottable/clearfilters/)() | يمسح جميع عوامل التصفية لهذا جدول المحور. |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle/)(PivotTable) | ينسخ النمط المسمى من جدول محور آخر. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose/)() | ينفّذ مهامًا معرفة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة تعيين الموارد غير المُدارة. |
| [ExportViewToJson](../../aspose.cells.pivot/pivottable/exportviewtojson/)(PivotViewToJsonOptions) | يصدّر عرض المحور كملف JSON. |
| [Fields](../../aspose.cells.pivot/pivottable/fields/)(PivotFieldType) | (**Obsolete.**) يحصل على الحقول المحددة حسب نوع الحقل. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format)(CellArea, Style) | يقوم بتنسيق المنطقة المحددة في جدول المحور. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_1)(PivotArea, Style) | يقوم بتنسيق المنطقة المحددة في جدول المحور. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_2)(int, int, Style) | يقوم بتنسيق الخلية في منطقة جدول المحور |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall/)(Style) | تنسيق جميع الخلايا في منطقة جدول المحور |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow/)(int, Style) | تنسيق بيانات الصف في منطقة جدول المحور |
| [GetButtonArea](../../aspose.cells.pivot/pivottable/getbuttonarea/)(PivotFieldType) | يحصل على المنطقة التي تحتوي على زر الحقل. |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname/)(string) | يحصل على كائن [`Cell`](../../aspose.cells/cell/) حسب الاسم المعروض لحقل المحور. |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren/)() | (**Obsolete.**) يحصل على جداول المحور الفرعية التي تستخدم بيانات جدول المحور هذا كمصدر بيانات. |
| [GetDependentPivotTables](../../aspose.cells.pivot/pivottable/getdependentpivottables/)() | يحصل على جميع `PivotTable`s التي تستخدم هذا جدول المحور كمصدر بيانات لها. |
| [GetFields](../../aspose.cells.pivot/pivottable/getfields/)(PivotFieldType) | يحصل على قائمة حقول المحور المحددة حسب المنطقة. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks/)() | (**Obsolete.**) يحصل على قائمة فهارس صفوف جدول المحور لفواصل الصفحات الأفقية |
| [GetHorizontalPageBreaks](../../aspose.cells.pivot/pivottable/gethorizontalpagebreaks/)() | يحصل على فواصل الصفحات الأفقية لهذا جدول المحور. |
| [GetNamesOfSourceDataConnections](../../aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/)() | يحصل على أسماء اتصالات بيانات المصدر الخارجي. |
| [GetPivotTablesWithSamePivotCache](../../aspose.cells.pivot/pivottable/getpivottableswithsamepivotcache/)() | يحصل على جميع جداول المحور التي تشترك في نفس ذاكرة التخزين المؤقت للمحور. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource)() | احصل على مصدر البيانات لهذا جدول المحور. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource_1)(bool) | احصل على مصدر البيانات لهذا جدول المحور. |
| [GetSourceDataConnections](../../aspose.cells.pivot/pivottable/getsourcedataconnections/)() | يحصل على مصادر بيانات الاتصالات الخارجية. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move_1)(string) | (**Obsolete.**) ينقل جدول المحور إلى موقع مختلف في ورقة العمل. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move)(int, int) | (**Obsolete.**) ينقل جدول المحور إلى موقع مختلف في ورقة العمل. |
| [MoveItem](../../aspose.cells.pivot/pivottable/moveitem/)(PivotFieldType, string[], bool, int) | انقل عنصرًا واحدًا للأعلى أو للأسفل. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_2)(string) | ينقل جدول المحور إلى موقع مختلف في ورقة العمل. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto)(int, int) | ينقل جدول المحور إلى موقع مختلف في ورقة العمل. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_1)(int, int, int) | ينقل جدول المحور إلى موقع مختلف في ورقة العمل. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh)() | تحديث [`PivotCache`](./pivotcache/) من مصدر البيانات وحساب البيانات والنمط لعرض المحور. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh_1)(PivotTableRefreshOption) | تحديث [`PivotCache`](./pivotcache/) من مصدر البيانات وحساب البيانات والنمط لعرض المحور. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata)() | (**Obsolete.**) يجدد البيانات من مصدرها إلى ذاكرة التخزين المؤقت للمحور. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata_1)(PivotTableRefreshOption) | (**Obsolete.**) يجدد بيانات جدول المحور وإعداداته من مصدرها مع الخيارات. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_1)(PivotFieldType, int) | يزيل حقلًا من منطقة المحور المحددة. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield)(PivotFieldType, PivotField) | إزالة الحقل من منطقة الحقل المحددة |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_2)(PivotFieldType, string) | يزيل حقلًا من منطقة الحقول المحددة |
| [SelectArea](../../aspose.cells.pivot/pivottable/selectarea/)(CellArea) | حدد منطقة من عرض جدول المحور. |
| [ShowDetail](../../aspose.cells.pivot/pivottable/showdetail/)(int, int, bool, int, int) | اعرض تفاصيل عنصر واحد في منطقة البيانات إلى جدول جديد. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform/)() | يصمم عرض PivotTable في شكل مدمج. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform/)() | يصمم PivotTable في شكل مخطط. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform/)() | يصمم PivotTable في شكل جدولي. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage/)(PivotField) | اعرض جميع صفحات مرشح التقرير وفقًا لـ PivotField، يجب أن يكون PivotField موجودًا في PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex/)(int) | اعرض جميع صفحات مرشح التقرير وفقًا لمؤشر الموقع في PageFields. |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname/)(string) | اعرض جميع صفحات مرشح التقرير وفقًا لاسم PivotField، يجب أن يكون PivotField موجودًا في PageFields. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotTableDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // تعيين بيانات عينة
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // إنشاء جدول محوري
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];

            // إضافة حقول
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // تنسيق جدول المحور
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // تخصيص حقل الصف
            PivotField rowField = pivot.RowFields[0];
            rowField.DisplayName = "Fruit Category";

            // تحديث وحساب البيانات
            pivot.RefreshData();
            pivot.CalculateData();

            // احفظ المصنف
            book.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


