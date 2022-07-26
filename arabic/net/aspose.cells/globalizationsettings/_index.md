---
title: GlobalizationSettings
second_title: Aspose.Cells لمرجع .NET API
description: يمثل إعدادات العولمة .
type: docs
weight: 3620
url: /ar/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

يمثل إعدادات العولمة .

```csharp
public class GlobalizationSettings : AbstractGlobalizationSettings
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [GlobalizationSettings](globalizationsettings)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings) { get; set; } | الحصول على المخطط أو تحديده[`ChartGlobalizationSettings`](../../aspose.cells.charts/chartglobalizationsettings) |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray) { get; } | يحصل على فاصل العناصر الموجودة في بيانات صف الصفيف في الصيغة. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator) { get; } | يحصل على فاصل القائمة ، معلمات الوظيفة ، ... الخ. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray) { get; } | يحصل على فاصل الصفوف في بيانات الصفيف في الصيغة. |

## طُرق

| اسم | وصف |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare)(string, string, bool) | مقارنة قيمتي سلسلة وفقًا لقواعد ترتيب معينة. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname)() | الحصول على اسم التسمية "(الكل)" في PivotTable. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring)(bool) | الحصول على قيمة سلسلة العرض للقيمة المنطقية للخلية |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey)(string, bool) | تحويل السلسلة إلى كائن قابل للمقارنة وفقًا لقواعد ترتيب معينة. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable)() | الحصول على اسم تسمية "عناوين الأعمدة" في PivotTable. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename)(CommentTitleType) | الحصول على اسم عنوان التعليق التابع للمنطقة المحلية وفقًا لنوع عنوان التعليق. |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname)() | الحصول على اسم التسمية "(فارغ)" في PivotTable. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring)(string) | الحصول على قيمة سلسلة العرض لقيمة خطأ الخلية value |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname)(ConsolidationFunction) | الحصول على الاسم الإجمالي الكلي للوظيفة. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname)(string) | الحصول على النص المعتمد على الإعدادات المحلية للاسم المضمن وفقًا للنص القياسي المحدد. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname)(string) | الحصول على اسم الوظيفة التابع للإعدادات المحلية وفقًا لاسم الوظيفة القياسي المحدد. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname)() | الحصول على اسم التسمية "(عناصر متعددة)" في PivotTable. |
| virtual [GetOtherName](../../aspose.cells/globalizationsettings/getothername)() | الحصول على اسم تسميات "أخرى" للمخططات الدائرية . |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname)() | الحصول على اسم تسمية "الإجمالي الكلي" في PivotTable. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname)() | الحصول على اسم التسمية "الإجمالي" في PivotTable. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي PivotTable على اثنين أو أكثر من حقول PivotField في منطقة البيانات. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable)() | الحصول على اسم الحماية في PivotTable . |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable)() | الحصول على اسم تسمية "عناوين الصفوف" في PivotTable. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname)(string) | الحصول على النص القياسي للاسم المضمن وفقًا للنص المعتمد على اللغة. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname)(string) | الحصول على اسم الوظيفة القياسي وفقًا لاسم الوظيفة المعتمدة على الإعدادات المحلية. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename)(string) | الحصول على اسم نمط الخط الإنجليزي القياسي (عادي ، غامق ، مائل) للرأس / التذييل وفقًا لاسم نمط الخط المحلي المحدد. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname)(PivotFieldSubtotalType) | يحصل على اسم[`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype) اكتب في PivotTable . |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall)() | الحصول على اسم نوع صفوف الجدول الذي يتكون من جميع الصفوف في الجدول المرجعي . القيمة الافتراضية هي "الكل" ، لذلك في الصيغة "#All" تمثل جميع الصفوف في الجدول المرجعي . |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent)() | الحصول على اسم نوع صفوف الجدول الذي يتكون من الصف الحالي في الجدول المشار إليه. الافتراضي هو "هذا الصف" ، لذلك في الصيغة "# هذا الصف" يمثل الصف الحالي في الجدول المرجعي . |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata)() | الحصول على اسم نوع صفوف الجدول التي تتكون من منطقة البيانات للجدول المرجعي. الافتراضي هو "البيانات" ، لذلك في الصيغة "#Data" تمثل منطقة البيانات في الجدول . |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders)() | الحصول على اسم نوع صفوف الجدول الذي يتكون من رأس الجدول. الافتراضي هو "رؤوس" ، لذلك في الصيغة "#Headers" يمثل رأس الجدول . |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals)() | الحصول على اسم نوع صفوف الجدول الذي يتكون من الصف الإجمالي للجدول المشار إليه. القيمة الافتراضية هي "الإجماليات" ، لذلك في الصيغة "# إجماليات" تمثل الصف الإجمالي للجدول المشار إليه. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname)(ConsolidationFunction) | الحصول على الاسم الإجمالي للوظيفة . |

### أنظر أيضا

* class [AbstractGlobalizationSettings](../abstractglobalizationsettings)
* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
