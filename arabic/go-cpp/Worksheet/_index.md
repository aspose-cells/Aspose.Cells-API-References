---
title: "فئة Worksheet"
linktitle: "Worksheet"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Worksheet. تغلف الكائن الذي يمثل ورقة العمل في Go."
type: docs
weight: 200
url: /ar/go-cpp/worksheet/
---

## Worksheet class

يحتوي على الكائن الذي يمثل ورقة عمل واحدة.

```go

type Worksheet struct  {
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
| [GetProtection](./getprotection/) | يمثل الأنواع المختلفة من خيارات الحماية المتاحة لورقة العمل. يدعم خيارات الحماية المتقدمة في ExcelXP والإصدارات الأحدث. |
| [GetUniqueId](./getuniqueid/) | يحصل على ويضبط المعرف الفريد، وهو نفسه {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [SetUniqueId](./setuniqueid/) | يحصل على ويضبط المعرف الفريد، وهو نفسه {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [GetPanes](./getpanes/) | يحصل على أقسام النافذة. |
| [GetWorkbook](./getworkbook/) | يحصل على كائن المصنف الذي يحتوي على هذه الورقة. |
| [GetCells](./getcells/) | يحصل على مجموعة Aspose.Cells.Cells. |
| [GetQueryTables](./getquerytables/) | يحصل على QueryTableCollection في ورقة العمل. |
| [GetType](./gettype/) | يمثل نوع ورقة العمل. |
| [SetType](./settype/) | يمثل نوع ورقة العمل. |
| [GetName](./getname/) | يحصل على أو يضبط اسم ورقة العمل. |
| [SetName](./setname/) | يحصل على أو يضبط اسم ورقة العمل. |
| [GetShowFormulas](./getshowformulas/) | يشير إلى ما إذا كان سيتم عرض الصيغ أو نتائجها. |
| [SetShowFormulas](./setshowformulas/) | يشير إلى ما إذا كان سيتم عرض الصيغ أو نتائجها. |
| [GetShowDataTypeIcons](./getshowdatatypeicons/) | يشير إلى ما إذا كان سيتم عرض أيقونات نوع البيانات. |
| [SetShowDataTypeIcons](./setshowdatatypeicons/) | يشير إلى ما إذا كان سيتم عرض أيقونات نوع البيانات. |
| [IsGridlinesVisible](./isgridlinesvisible/) | يحصل على أو يضبط قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true. |
| [SetIsGridlinesVisible](./setisgridlinesvisible/) | يحصل على أو يضبط قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true. |
| [IsRowColumnHeadersVisible](./isrowcolumnheadersvisible/) | يحصل على أو يضبط قيمة تشير إلى ما إذا كانت ورقة العمل ستعرض رؤوس الصفوف والأعمدة. القيمة الافتراضية هي true. |
| [SetIsRowColumnHeadersVisible](./setisrowcolumnheadersvisible/) | يحصل على أو يضبط قيمة تشير إلى ما إذا كانت ورقة العمل ستعرض رؤوس الصفوف والأعمدة. القيمة الافتراضية هي true. |
| [GetPaneState](./getpanestate/) | يشير إلى ما إذا كان القسم يحتوي على تقسيمات أفقية أو عمودية، وما إذا كانت تلك التقسيمات مجمدة. |
| [GetDisplayZeros](./getdisplayzeros/) | صحيح إذا تم عرض القيم الصفرية. |
| [SetDisplayZeros](./setdisplayzeros/) | صحيح إذا تم عرض القيم الصفرية. |
| [GetDisplayRightToLeft](./getdisplayrighttoleft/) | يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. القيمة الافتراضية هي false. |
| [SetDisplayRightToLeft](./setdisplayrighttoleft/) | يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. القيمة الافتراضية هي false. |
| [IsOutlineShown](./isoutlineshown/) | يشير إلى ما إذا كان سيتم عرض المخطط. |
| [SetIsOutlineShown](./setisoutlineshown/) | يشير إلى ما إذا كان سيتم عرض المخطط. |
| [IsSelected](./isselected/) | يشير إلى ما إذا كانت ورقة العمل هذه مختارة عند فتح المصنف. |
| [SetIsSelected](./setisselected/) | يشير إلى ما إذا كانت ورقة العمل هذه مختارة عند فتح المصنف. |
| [FreezePanes_Int_Int_Int_Int](./freezepanes_int_int_int_int/) | يقوم بتجميد الأقسام عند الخلية المحددة في ورقة العمل. |
| [GetFreezedPanes](./getfreezedpanes/) | يحصل على تجميد الأقسام. |
| [Split](./split/) | يقسم النافذة. |
| [FreezePanes_String_Int_Int](./freezepanes_string_int_int/) | يقوم بتجميد الأقسام عند الخلية المحددة في ورقة العمل. |
| [UnFreezePanes](./unfreezepanes/) | يفك تجميد الأقسام في ورقة العمل. |
| [RemoveSplit](./removesplit/) | يزيل تقسيم النافذة. |
| [GetPivotTables](./getpivottables/) | يحصل على جميع جداول المحور في هذه الورقة. |
| [GetListObjects](./getlistobjects/) | يحصل على جميع ListObjects في هذه الورقة. |
| [GetTabId](./gettabid/) | يحدد المعرف الداخلي للورقة. |
| [SetTabId](./settabid/) | يحدد المعرف الداخلي للورقة. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | يحصل على مجموعة HorizontalPageBreakCollection. |
| [GetVerticalPageBreaks](./getverticalpagebreaks/) | يحصل على مجموعة VerticalPageBreakCollection. |
| [AddPageBreaks](./addpagebreaks/) | يضيف فاصل صفحة. |
| [GetHyperlinks](./gethyperlinks/) | يحصل على مجموعة HyperlinkCollection. |
| [Copy_Worksheet](./copy_worksheet/) | ينسخ المحتويات والتنسيقات من ورقة عمل أخرى. |
| [Copy_Worksheet_CopyOptions](./copy_worksheet_copyoptions/) | ينسخ المحتويات والتنسيقات من ورقة عمل أخرى. |
| [AutoFitColumn_Int_Int_Int](./autofitcolumn_int_int_int/) | يضبط عرض العمود تلقائيًا. |
| [AutoFitColumns](./autofitcolumns/) | يضبط جميع الأعمدة في ورقة العمل هذه تلقائيًا. |
| [AutoFitColumns_AutoFitterOptions](./autofitcolumns_autofitteroptions/) | يضبط جميع الأعمدة في ورقة العمل هذه تلقائيًا. |
| [AutoFitColumn_Int](./autofitcolumn_int/) | يضبط عرض العمود تلقائيًا. |
| [AutoFitColumns_Int_Int](./autofitcolumns_int_int/) | يضبط عرض الأعمدة تلقائيًا. |
| [AutoFitColumns_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_autofitteroptions/) | يضبط عرض الأعمدة تلقائيًا. |
| [AutoFitColumns_Int_Int_Int_Int](./autofitcolumns_int_int_int_int/) | يضبط عرض الأعمدة تلقائيًا. |
| [AutoFitColumns_Int_Int_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_int_int_autofitteroptions/) | يضبط عرض الأعمدة تلقائيًا. |
| [AutoFitRow_Int_Int_Int](./autofitrow_int_int_int/) | يضبط ارتفاع الصف تلقائيًا. |
| [AutoFitRow_Int_Int_Int_AutoFitterOptions](./autofitrow_int_int_int_autofitteroptions/) | يضبط ارتفاع الصف تلقائيًا. |
| [AutoFitRows](./autofitrows/) | يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا. |
| [AutoFitRows_Bool](./autofitrows_bool/) | يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا. |
| [AutoFitRows_AutoFitterOptions](./autofitrows_autofitteroptions/) | يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا. |
| [AutoFitRows_Int_Int](./autofitrows_int_int/) | يضبط ارتفاع الصف في نطاق تلقائيًا. |
| [AutoFitRows_Int_Int_AutoFitterOptions](./autofitrows_int_int_autofitteroptions/) | يضبط ارتفاع الصف في نطاق تلقائيًا. |
| [AutoFitRow_Int_Int_Int_Int](./autofitrow_int_int_int_int/) | يضبط ارتفاع الصف في نطاق مستطيل تلقائيًا. |
| [AutoFitRow_Int](./autofitrow_int/) | يضبط ارتفاع الصف تلقائيًا. |
| [GetPageSetup](./getpagesetup/) | يمثل وصف إعداد الصفحة في هذه الورقة. |
| [GetAutoFilter](./getautofilter/) | يمثل الفلتر التلقائي للورقة المحددة. |
| [Filter](./filter/) | يفلتر النطاق. |
| [GetAdvancedFilter](./getadvancedfilter/) | يحصل على إعدادات الفلتر المتقدم. |
| [Advanced_Filter](./advanced_filter/) | يفلتر البيانات باستخدام معايير معقدة. |
| [RemoveAutoFilter](./removeautofilter/) | يزيل الفلتر التلقائي للورقة. |
| [GetHasAutofilter](./gethasautofilter/) | يشير إلى ما إذا كانت هذه الورقة تحتوي على فلتر تلقائي. |
| [GetTransitionEvaluation](./gettransitionevaluation/) | يشير إلى ما إذا كان خيار تقييم صيغ الانتقال (توافق Lotus) مفعلاً. |
| [SetTransitionEvaluation](./settransitionevaluation/) | يشير إلى ما إذا كان خيار تقييم صيغ الانتقال (توافق Lotus) مفعلاً. |
| [GetTransitionEntry](./gettransitionentry/) | يشير إلى ما إذا كان خيار إدخال صيغ الانتقال (توافق Lotus) مفعلاً. |
| [SetTransitionEntry](./settransitionentry/) | يشير إلى ما إذا كان خيار إدخال صيغ الانتقال (توافق Lotus) مفعلاً. |
| [GetVisibilityType](./getvisibilitytype/) | يشير إلى الحالة المرئية لهذه الورقة. |
| [SetVisibilityType](./setvisibilitytype/) | يشير إلى الحالة المرئية لهذه الورقة. |
| [SetVisible](./setvisible/) | يضبط الخيارات المرئية. |
| [IsVisible](./isvisible/) | يمثل ما إذا كانت الورقة مرئية. |
| [SetIsVisible](./setisvisible/) | يمثل ما إذا كانت الورقة مرئية. |
| [SelectRange](./selectrange/) | يحدد نطاقًا. |
| [RemoveAllDrawingObjects](./removealldrawingobjects/) | يزيل جميع كائنات الرسم في هذه ورقة العمل. |
| [ClearComments](./clearcomments/) | يمسح جميع التعليقات في جدول البيانات المصمم. |
| [GetSparklineGroups](./getsparklinegroups/) | يحصل على مجموعات السباركلين في ورقة العمل. |
| [GetCharts](./getcharts/) | يحصل على مجموعة المخططات |
| [GetComments](./getcomments/) | يحصل على مجموعة التعليقات. |
| [GetPictures](./getpictures/) | يحصل على مجموعة الصور. |
| [GetAllPictures](./getallpictures/) | يحصل على جميع الصور بما في ذلك الصور المدمجة في الخلية والتي فوق الخلايا. |
| [GetTextBoxes](./gettextboxes/) | يحصل على مجموعة صناديق النص. |
| [GetCheckBoxes](./getcheckboxes/) | يحصل على مجموعة مربعات الاختيار. |
| [GetOleObjects](./getoleobjects/) | يمثل مجموعة من OleObject في ورقة العمل. |
| [GetShapes](./getshapes/) | يرجع جميع أشكال الرسم في هذه ورقة العمل. |
| [GetSlicers](./getslicers/) | احصل على مجموعة الشرائح في ورقة العمل |
| [GetTimelines](./gettimelines/) | احصل على مجموعة المخطط الزمني في ورقة العمل |
| [Protect_ProtectionType](./protect_protectiontype/) | يحمي ورقة العمل. |
| [Protect_ProtectionType_String_String](./protect_protectiontype_string_string/) | يحمي ورقة العمل. |
| [Unprotect](./unprotect/) | يلغي حماية ورقة العمل. |
| [Unprotect_String](./unprotect_string/) | يلغي حماية ورقة العمل. |
| [GetIndex](./getindex/) | يحصل على فهرس الورقة في مجموعة أوراق العمل. |
| [MoveTo](./moveto/) | ينقل الورقة إلى موقع آخر في جدول البيانات. |
| [IsProtected](./isprotected/) | يشير إلى ما إذا كانت ورقة العمل محمية. |
| [GetValidations](./getvalidations/) | يحصل على مجموعة إعدادات التحقق من البيانات في ورقة العمل. |
| [GetAllowEditRanges](./getalloweditranges/) | يحصل على مجموعة نطاقات السماح بالتحرير في ورقة العمل. |
| [GetErrorCheckOptions](./geterrorcheckoptions/) | يحصل على إعداد فحص الأخطاء المطبق على نطاقات معينة. |
| [GetOutline](./getoutline/) | يحصل على المخطط التفصيلي في هذه ورقة العمل. |
| [GetFirstVisibleRow](./getfirstvisiblerow/) | يمثل فهرس الصف الأول المرئي. |
| [SetFirstVisibleRow](./setfirstvisiblerow/) | يمثل فهرس الصف الأول المرئي. |
| [GetFirstVisibleColumn](./getfirstvisiblecolumn/) | يمثل فهرس العمود الأول المرئي. |
| [SetFirstVisibleColumn](./setfirstvisiblecolumn/) | يمثل فهرس العمود الأول المرئي. |
| [Replace](./replace/) | يستبدل نص جميع الخلايا بسلسلة جديدة. |
| [GetZoom](./getzoom/) | يمثل معامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400. |
| [SetZoom](./setzoom/) | يمثل معامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400. |
| [GetViewType](./getviewtype/) | يحصل على نوع العرض ويضبطه. |
| [SetViewType](./setviewtype/) | يحصل على نوع العرض ويضبطه. |
| [IsPageBreakPreview](./ispagebreakpreview/) | يشير إلى ما إذا كانت ورقة العمل المحددة معروضة في العرض العادي أو معاينة فواصل الصفحات. |
| [SetIsPageBreakPreview](./setispagebreakpreview/) | يشير إلى ما إذا كانت ورقة العمل المحددة معروضة في العرض العادي أو معاينة فواصل الصفحات. |
| [IsRulerVisible](./isrulervisible/) | يشير إلى ما إذا كان المسطر يظهر. يتم تطبيق هذه الخاصية فقط في معاينة فواصل الصفحات. |
| [SetIsRulerVisible](./setisrulervisible/) | يشير إلى ما إذا كان المسطر يظهر. يتم تطبيق هذه الخاصية فقط في معاينة فواصل الصفحات. |
| [GetSelectedAreas](./getselectedareas/) | يحصل على النطاقات المحددة من الخلايا في جدول البيانات المصمم. |
| [GetTabColor](./gettabcolor/) | يمثل لون تبويب ورقة العمل. |
| [SetTabColor](./settabcolor/) | يمثل لون تبويب ورقة العمل. |
| [GetGridlineColor](./getgridlinecolor/) | يحصل على لون خطوط الشبكة ويضبطه |
| [SetGridlineColor](./setgridlinecolor/) | يحصل على لون خطوط الشبكة ويضبطه |
| [GetCodeName](./getcodename/) | يحصل على الاسم الرمزي لورقة العمل. |
| [SetCodeName](./setcodename/) | يحصل على الاسم الرمزي لورقة العمل. |
| [GetBackgroundImage](./getbackgroundimage/) | يحصل على صورة خلفية ورقة العمل ويضبطها. |
| [SetBackgroundImage](./setbackgroundimage/) | يحصل على صورة خلفية ورقة العمل ويضبطها. |
| [GetConditionalFormattings](./getconditionalformattings/) | يحصل على تنسيقات الشرطية في ورقة العمل. |
| [GetActiveCell](./getactivecell/) | يحصل على الخلية النشطة في ورقة العمل أو يضبطها. |
| [SetActiveCell](./setactivecell/) | يحصل على الخلية النشطة في ورقة العمل أو يضبطها. |
| [GetCustomProperties](./getcustomproperties/) | يحصل على كائن يمثل معلومات المعرف المرتبطة بورقة عمل. |
| [GetPrintingPageBreaks](./getprintingpagebreaks/) | يحصل على فواصل الصفحات التلقائية. |
| [GetSmartTagSetting](./getsmarttagsetting/) | يحصل على جميع كائنات SmartTagCollection في ورقة العمل. |
| [ToString](./tostring/) | يرجع سلسلة تمثل كائن ورقة العمل الحالي. |
| [GetScenarios](./getscenarios/) | يحصل على مجموعة السيناريوهات. |
| [StartAccessCache](./startaccesscache/) | يبدأ الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات في هذه الورقة. |
| [CloseAccessCache](./closeaccesscache/) | يغلق الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات في هذه الورقة. |
| [ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | يحول نمط إشارة الصيغة. |
| [CalculateFormula_String](./calculateformula_string/) | يحسب صيغة. |
| [CalculateFormula_String_CalculationOptions](./calculateformula_string_calculationoptions/) | يحسب تعبير الصيغة مباشرة. |
| [CalculateFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_CalculationData](./calculateformula_string_formulaparseoptions_calculationoptions_int_int_calculationdata/) | يحسب تعبير الصيغة مباشرة. |
| [CalculateArrayFormula_String_CalculationOptions](./calculatearrayformula_string_calculationoptions/) | يحسب الصيغة كصيغة مصفوفية. |
| [CalculateArrayFormula_String_CalculationOptions_Int_Int](./calculatearrayformula_string_calculationoptions_int_int/) | يحسب الصيغة كصيغة مصفوفية. |
| [CalculateArrayFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_Int_Int_CalculationData](./calculatearrayformula_string_formulaparseoptions_calculationoptions_int_int_int_int_calculationdata/) | يحسب الصيغة كصيغة مصفوفية. |
| [CalculateFormula_CalculationOptions_Bool](./calculateformula_calculationoptions_bool/) | يحسب جميع الصيغ في هذه الورقة. |
| [GetAreasOfXmlMapQuery](./getareasofxmlmapquery/) | استعلام عن مناطق الخلايا التي تم ربطها/ربطها بالمسار المحدد لخريطة XML. |
| [GetCellWatches](./getcellwatches/) | يحصل على مجموعة الخلايا في هذه ورقة العمل التي يتم مراقبتها في 'نافذة المراقبة'. |
| [RefreshPivotTables](./refreshpivottables/) | يقوم بتحديث جميع جداول Pivot في هذه ورقة العمل. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | يقوم بتحديث جميع جداول Pivot في هذه ورقة العمل. |
