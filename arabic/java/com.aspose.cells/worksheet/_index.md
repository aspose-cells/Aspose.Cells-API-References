---
title: "Worksheet"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل ورقة عمل واحدة."
type: docs
url: /ar/java/com.aspose.cells/worksheet/
---

**Inheritance:**
java.lang.Object
```
public class Worksheet
```

يغلف الكائن الذي يمثل ورقة عمل واحدة.

**Example**

المثال التالي يوضح كيفية تجميد الألواح وإدراج رابط تشعبي إلى ورقة العمل باستخدام .Net أو VB.

```
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Freeze panes at "AS40" with 10 rows and 10 columns
         sheet.freezePanes("AS40", 10, 10);
 
         //Add a hyperlink in Cell A1
         sheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addPageBreaks(String cellName)](#addPageBreaks-java.lang.String-) | يضيف فاصل صفحة. |
| [advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)](#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-) | يقوم بتصفية البيانات باستخدام معايير معقدة. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | يضبط عرض العمود تلقائيًا. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | يضبط عرض العمود تلقائيًا. |
| [autoFitColumns()](#autoFitColumns--) | يضبط جميع الأعمدة في ورقة العمل هذه تلقائيًا. |
| [autoFitColumns(AutoFitterOptions options)](#autoFitColumns-com.aspose.cells.AutoFitterOptions-) | يضبط جميع الأعمدة في ورقة العمل هذه تلقائيًا. |
| [autoFitColumns(int firstColumn, int lastColumn)](#autoFitColumns-int-int-) | يضبط عرض الأعمدة تلقائيًا. |
| [autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-) | يضبط عرض الأعمدة تلقائيًا. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)](#autoFitColumns-int-int-int-int-) | يضبط عرض الأعمدة تلقائيًا. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-) | يضبط عرض الأعمدة تلقائيًا. |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | يضبط ارتفاع الصف تلقائيًا. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | يضبط ارتفاع الصف تلقائيًا. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-) | يضبط ارتفاع الصف تلقائيًا. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | يضبط ارتفاع الصف في نطاق مستطيل تلقائيًا. |
| [autoFitRows()](#autoFitRows--) | يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا. |
| [autoFitRows(AutoFitterOptions options)](#autoFitRows-com.aspose.cells.AutoFitterOptions-) | يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | يضبط ارتفاع الصف في نطاق تلقائيًا. |
| [autoFitRows(int startRow, int endRow, AutoFitterOptions options)](#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-) | يضبط ارتفاع الصف في نطاق تلقائيًا. |
| [calculateArrayFormula(String formula, CalculationOptions opts)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | يحسب صيغة كصيغة مصفوفة. |
| [calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-) | يحسب صيغة كصيغة مصفوفة. |
| [calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)](#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-) | يحسب صيغة كصيغة مصفوفة. |
| [calculateFormula(CalculationOptions options, boolean recursive)](#calculateFormula-com.aspose.cells.CalculationOptions-boolean-) | يحسب جميع الصيغ في ورقة العمل هذه. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | يحسب صيغة. |
| [calculateFormula(String formula, CalculationOptions opts)](#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | يحسب تعبير الصيغة مباشرة. |
| [calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)](#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-) | يحسب تعبير الصيغة مباشرة. |
| [clearComments()](#clearComments--) | يمسح جميع التعليقات في جدول البيانات المصمم. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | يغلق الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات في ورقة العمل هذه. |
| [convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)](#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-) | يحول نمط مرجع الصيغة. |
| [copy(Worksheet sourceSheet)](#copy-com.aspose.cells.Worksheet-) | ينسخ المحتويات والتنسيقات من ورقة عمل أخرى. |
| [copy(Worksheet sourceSheet, CopyOptions copyOptions)](#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-) | ينسخ المحتويات والتنسيقات من ورقة عمل أخرى. |
| [dispose()](#dispose--) | ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(CellArea ca)](#filter-com.aspose.cells.CellArea-) | يقوم بتصفية النطاق. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | يثبت الألواح عند الخلية المحددة في ورقة العمل. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | يثبت الألواح عند الخلية المحددة في ورقة العمل. |
| [getActiveCell()](#getActiveCell--) | يحصل على الخلية النشطة في ورقة العمل. |
| [getAdvancedFilter()](#getAdvancedFilter--) | يحصل على إعدادات الفلتر المتقدم. |
| [getAllPictures()](#getAllPictures--) | يحصل على جميع الصور بما في ذلك الصور المدمجة في الخلية وفوق الخلايا. |
| [getAllowEditRanges()](#getAllowEditRanges--) | يحصل على مجموعة نطاقات السماح بالتعديل في ورقة العمل. |
| [getAreasOfXmlMapQuery(String path, XmlMap xmlMap)](#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | يستعلم عن مناطق الخلايا التي تم ربطها/ربطها بالمسار المحدد لخريطة XML. |
| [getAutoFilter()](#getAutoFilter--) | يمثل الفلتر التلقائي لورقة العمل المحددة. |
| [getBackgroundImage()](#getBackgroundImage--) | يحصل على صورة خلفية ورقة العمل. |
| [getCellWatches()](#getCellWatches--) | يحصل على مجموعة الخلايا في هذه ورقة العمل التي يتم مراقبتها في 'نافذة المراقبة'. |
| [getCells()](#getCells--) | يحصل على مجموعة [Cells](../../com.aspose.cells/cells). |
| [getCharts()](#getCharts--) | يحصل على مجموعة [Chart](../../com.aspose.cells/chart) |
| [getCheckBoxes()](#getCheckBoxes--) | يحصل على مجموعة [CheckBox](../../com.aspose.cells/checkbox). |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | يحصل على اسم رمز ورقة العمل. |
| [getComments()](#getComments--) | يحصل على مجموعة [Comment](../../com.aspose.cells/comment). |
| [getConditionalFormattings()](#getConditionalFormattings--) | يحصل على ConditionalFormattings في ورقة العمل. |
| [getCustomProperties()](#getCustomProperties--) | يحصل على كائن يمثل معلومات المعرف المرتبطة بورقة عمل. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. |
| [getDisplayZeros()](#getDisplayZeros--) | صحيح إذا تم عرض القيم الصفرية. |
| [getErrorCheckOptions()](#getErrorCheckOptions--) | يحصل على إعداد فحص الأخطاء المطبق على نطاقات معينة. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | يمثل فهرس العمود الأول الظاهر. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | يمثل فهرس الصف الأول الظاهر. |
| [getFreezedPanes()](#getFreezedPanes--) | يحصل على تجميد الألواح. |
| [getGridlineColor()](#getGridlineColor--) | يحصل على لون خط الشبكة |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | يحصل على مجموعة [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection). |
| [getHyperlinks()](#getHyperlinks--) | يحصل على مجموعة [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection). |
| [getIndex()](#getIndex--) | يحصل على فهرس الورقة في مجموعة أوراق العمل. |
| [getListObjects()](#getListObjects--) | يحصل على جميع ListObjects في هذه ورقة العمل. |
| [getName()](#getName--) | يحصل على اسم ورقة العمل. |
| [getOleObjects()](#getOleObjects--) | يمثل مجموعة من [OleObject](../../com.aspose.cells/oleobject) في ورقة عمل. |
| [getOutline()](#getOutline--) | يحصل على المخطط التفصيلي في هذه ورقة العمل. |
| [getPageSetup()](#getPageSetup--) | يمثل وصف إعداد الصفحة في هذه الورقة. |
| [getPaneState()](#getPaneState--) | يشير إلى ما إذا كان الجزء يحتوي على تقسيمات أفقية أو عمودية، وما إذا كانت تلك التقسيمات مجمدة. |
| [getPanes()](#getPanes--) | يحصل على أجزاء النافذة. |
| [getPictures()](#getPictures--) | يحصل على مجموعة [Picture](../../com.aspose.cells/picture). |
| [getPivotTables()](#getPivotTables--) | يحصل على جميع جداول المحور في هذه ورقة العمل. |
| [getPrintingPageBreaks(ImageOrPrintOptions options)](#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-) | يحصل على فواصل الصفحات التلقائية. |
| [getProtection()](#getProtection--) | يمثل الأنواع المختلفة لخيارات الحماية المتاحة لورقة العمل. |
| [getQueryTables()](#getQueryTables--) | يحصل على [QueryTableCollection](../../com.aspose.cells/querytablecollection) في ورقة العمل. |
| [getScenarios()](#getScenarios--) | يحصل على مجموعة [Scenario](../../com.aspose.cells/scenario). |
| [getSelectedAreas()](#getSelectedAreas--) | يحصل على النطاقات المحددة من الخلايا في جدول البيانات المصمم. |
| [getSelectedRanges()](#getSelectedRanges--) | يحصل على النطاقات المحددة من الخلايا في جدول البيانات المصمم. |
| [getShapes()](#getShapes--) | يعيد جميع أشكال الرسم في هذه ورقة العمل. |
| [getShowDataTypeIcons()](#getShowDataTypeIcons--) | يشير إلى ما إذا كان يجب إظهار أيقونات نوع البيانات. |
| [getShowFormulas()](#getShowFormulas--) | يشير إلى ما إذا كان يجب إظهار الصيغ أو نتائجها. |
| [getSlicers()](#getSlicers--) | احصل على مجموعة Slicer في ورقة العمل |
| [getSmartTagSetting()](#getSmartTagSetting--) | يحصل على جميع كائنات [SmartTagCollection](../../com.aspose.cells/smarttagcollection) في ورقة العمل. |
| [getSparklineGroups()](#getSparklineGroups--) | يحصل على مجموعات sparkline في ورقة العمل. |
| [getTabColor()](#getTabColor--) | يمثل لون تبويب ورقة العمل. |
| [getTabId()](#getTabId--) | يحدد المعرف الداخلي للورقة. |
| [getTextBoxes()](#getTextBoxes--) | يحصل على مجموعة [TextBox](../../com.aspose.cells/textbox). |
| [getTimelines()](#getTimelines--) | احصل على مجموعة Timeline في ورقة العمل |
| [getTransitionEntry()](#getTransitionEntry--) | يشير إلى ما إذا كان خيار إدخال صيغة الانتقال (توافق Lotus) مفعلاً. |
| [getTransitionEvaluation()](#getTransitionEvaluation--) | يشير إلى ما إذا كان خيار تقييم صيغة الانتقال (توافق Lotus) مفعلاً. |
| [getType()](#getType--) | يمثل نوع ورقة العمل. |
| [getUniqueId()](#getUniqueId--) | يحصل على المعرف الفريد، وهو نفسه \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [getValidations()](#getValidations--) | يحصل على مجموعة إعدادات التحقق من صحة البيانات في ورقة العمل. |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--) | يحصل على مجموعة [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection). |
| [getViewType()](#getViewType--) | يحصل على نوع العرض. |
| [getVisibilityType()](#getVisibilityType--) | يشير إلى الحالة المرئية لهذه الورقة. |
| [getWorkbook()](#getWorkbook--) | يحصل على كائن المصنف الذي يحتوي على هذه الورقة. |
| [getZoom()](#getZoom--) | يمثل عامل التحجيم بالنسبة المئوية. |
| [hasAutofilter()](#hasAutofilter--) | يشير إلى ما إذا كانت هذه ورقة العمل تحتوي على مرشح تلقائي. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | يحصل على قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true. |
| [isOutlineShown()](#isOutlineShown--) | يشير إلى ما إذا كان يجب إظهار المخطط. |
| [isPageBreakPreview()](#isPageBreakPreview--) | يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض في العرض العادي أو معاينة فواصل الصفحات. |
| [isProtected()](#isProtected--) | يشير إلى ما إذا كانت ورقة العمل محمية. |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--) | يحصل على قيمة تشير إلى ما إذا كانت ورقة العمل ستعرض رؤوس الصفوف والأعمدة. |
| [isRulerVisible()](#isRulerVisible--) | يشير إلى ما إذا كان المسطرة مرئية. |
| [isSelected()](#isSelected--) | يشير إلى ما إذا كانت ورقة العمل هذه مختارة عند فتح دفتر العمل. |
| [isVisible()](#isVisible--) | يمثل ما إذا كانت ورقة العمل مرئية. |
| [moveTo(int index)](#moveTo-int-) | ينقل الورقة إلى موقع آخر في جدول البيانات. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(int type)](#protect-int-) | يحمي ورقة العمل. |
| [protect(int type, String password, String oldPassword)](#protect-int-java.lang.String-java.lang.String-) | يحمي ورقة العمل. |
| [refreshPivotTables()](#refreshPivotTables--) | يقوم بتحديث جميع جداول PivotTables في هذه ورقة العمل. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | يقوم بتحديث جميع جداول PivotTables في هذه ورقة العمل. |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--) | يزيل جميع كائنات الرسم في هذه ورقة العمل. |
| [removeAutoFilter()](#removeAutoFilter--) | يزيل المرشح التلقائي لورقة العمل. |
| [removeSplit()](#removeSplit--) | يزيل تقسيم النافذة. |
| [replace(String oldString, String newString)](#replace-java.lang.String-java.lang.String-) | يستبدل نص جميع الخلايا بسلسلة جديدة. |
| [selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)](#selectRange-int-int-int-int-boolean-) | يحدد نطاقًا. |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | يضبط الخلية النشطة في ورقة العمل. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | يضبط صورة خلفية ورقة العمل. |
| [setCodeName(String value)](#setCodeName-java.lang.String-) | يحصل على اسم رمز ورقة العمل. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | صحيح إذا تم عرض القيم الصفرية. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | يمثل فهرس العمود الأول الظاهر. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | يمثل فهرس الصف الأول الظاهر. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | يضبط لون خط الشبكة |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | يضبط قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم ورقة العمل. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | يشير إلى ما إذا كان يجب إظهار المخطط. |
| [setPageBreakPreview(boolean value)](#setPageBreakPreview-boolean-) | يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض في العرض العادي أو معاينة فواصل الصفحات. |
| [setRowColumnHeadersVisible(boolean value)](#setRowColumnHeadersVisible-boolean-) | يضبط قيمة تشير إلى ما إذا كانت ورقة العمل ستعرض رؤوس الصفوف والأعمدة. |
| [setRulerVisible(boolean value)](#setRulerVisible-boolean-) | يشير إلى ما إذا كان المسطرة مرئية. |
| [setSelected(boolean value)](#setSelected-boolean-) | يشير إلى ما إذا كانت ورقة العمل هذه مختارة عند فتح دفتر العمل. |
| [setShowDataTypeIcons(boolean value)](#setShowDataTypeIcons-boolean-) | يشير إلى ما إذا كان يجب إظهار أيقونات نوع البيانات. |
| [setShowFormulas(boolean value)](#setShowFormulas-boolean-) | يشير إلى ما إذا كان يجب إظهار الصيغ أو نتائجها. |
| [setTabColor(Color value)](#setTabColor-com.aspose.cells.Color-) | يمثل لون تبويب ورقة العمل. |
| [setTabId(int value)](#setTabId-int-) | يحدد المعرف الداخلي للورقة. |
| [setTransitionEntry(boolean value)](#setTransitionEntry-boolean-) | يشير إلى ما إذا كان خيار إدخال صيغة الانتقال (توافق Lotus) مفعلاً. |
| [setTransitionEvaluation(boolean value)](#setTransitionEvaluation-boolean-) | يشير إلى ما إذا كان خيار تقييم صيغة الانتقال (توافق Lotus) مفعلاً. |
| [setType(int value)](#setType-int-) | يمثل نوع ورقة العمل. |
| [setUniqueId(String value)](#setUniqueId-java.lang.String-) | يضبط المعرف الفريد، وهو نفسه \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [setViewType(int value)](#setViewType-int-) | يضبط نوع العرض. |
| [setVisibilityType(int value)](#setVisibilityType-int-) | يشير إلى الحالة المرئية لهذه الورقة. |
| [setVisible(boolean value)](#setVisible-boolean-) | يمثل ما إذا كانت ورقة العمل مرئية. |
| [setVisible(boolean isVisible, boolean ignoreError)](#setVisible-boolean-boolean-) | يضبط الخيارات المرئية. |
| [setZoom(int value)](#setZoom-int-) | يمثل عامل التحجيم بالنسبة المئوية. |
| [split()](#split--) | يقسم النافذة. |
| [startAccessCache(int opts)](#startAccessCache-int-) | يبدأ الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات في ورقة العمل هذه. |
| [toString()](#toString--) | يرجع سلسلة تمثل كائن ورقة العمل الحالي. |
| [unFreezePanes()](#unFreezePanes--) | يفك تجميد الألواح في ورقة العمل. |
| [unprotect()](#unprotect--) | يلغي حماية ورقة العمل. |
| [unprotect(String password)](#unprotect-java.lang.String-) | يلغي حماية ورقة العمل. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [xmlMapQuery(String path, XmlMap xmlMap)](#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | يستعلم عن مناطق الخلايا التي تم ربطها/ربطها بالمسار المحدد لخريطة XML. |
### addPageBreaks(String cellName) {#addPageBreaks-java.lang.String-}
```
public void addPageBreaks(String cellName)
```


يضيف فاصل صفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String |  |

### advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly) {#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public void advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)
```


يقوم بتصفية البيانات باستخدام معايير معقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isFilter | boolean | يشير إلى ما إذا كان يتم تصفية القائمة في مكانها. |
| listRange | java.lang.String | نطاق القائمة. |
| criteriaRange | java.lang.String | نطاق المعايير. |
| copyTo | java.lang.String | النطاق الذي يتم النسخ إليه. |
| uniqueRecordOnly | boolean | عرض أو نسخ الصفوف الفريدة فقط. |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


يضبط عرض العمود تلقائيًا.

**Remarks**

AutoFitColumn هي دالة غير دقيقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


يضبط عرض العمود تلقائيًا.

**Remarks**

تقوم هذه الطريقة بضبط عرض الصف تلقائيًا بناءً على المحتوى في نطاق الخلايا داخل الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |
| firstRow | int | فهرس الصف الأول. |
| lastRow | int | فهرس الصف الأخير. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```


يضبط جميع الأعمدة في ورقة العمل هذه تلقائيًا.

### autoFitColumns(AutoFitterOptions options) {#autoFitColumns-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(AutoFitterOptions options)
```


يضبط جميع الأعمدة في ورقة العمل هذه تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | خيارات الضبط التلقائي |

### autoFitColumns(int firstColumn, int lastColumn) {#autoFitColumns-int-int-}
```
public void autoFitColumns(int firstColumn, int lastColumn)
```


يضبط عرض الأعمدة تلقائيًا.

**Remarks**

AutoFitColumn هي دالة غير دقيقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstColumn | int | فهرس العمود الأول. |
| lastColumn | int | فهرس العمود الأخير. |

### autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```


يضبط عرض الأعمدة تلقائيًا.

**Remarks**

AutoFitColumn هي دالة غير دقيقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstColumn | int | فهرس العمود الأول. |
| lastColumn | int | فهرس العمود الأخير. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | خيارات الضبط التلقائي |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn) {#autoFitColumns-int-int-int-int-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```


يضبط عرض الأعمدة تلقائيًا.

**Remarks**

AutoFitColumn هي دالة غير دقيقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | فهرس الصف الأول. |
| firstColumn | int | فهرس العمود الأول. |
| lastRow | int | فهرس الصف الأخير. |
| lastColumn | int | فهرس العمود الأخير. |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)
```


يضبط عرض الأعمدة تلقائيًا.

**Remarks**

AutoFitColumn هي دالة غير دقيقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | فهرس الصف الأول. |
| firstColumn | int | فهرس العمود الأول. |
| lastRow | int | فهرس الصف الأخير. |
| lastColumn | int | فهرس العمود الأخير. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | خيارات الضبط التلقائي |

### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


يضبط ارتفاع الصف تلقائيًا.

**Remarks**

AutoFitRow هي دالة غير دقيقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


يضبط ارتفاع الصف تلقائيًا.

**Remarks**

تقوم هذه الطريقة بضبط عرض الصف تلقائيًا بناءً على المحتوى في نطاق الخلايا داخل الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |
| firstColumn | int | فهرس العمود الأول. |
| lastColumn | int | فهرس العمود الأخير. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```


يضبط ارتفاع الصف تلقائيًا.

**Remarks**

تقوم هذه الطريقة بضبط عرض الصف تلقائيًا بناءً على المحتوى في نطاق الخلايا داخل الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |
| firstColumn | int | فهرس العمود الأول. |
| lastColumn | int | فهرس العمود الأخير. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | خيارات الضبط التلقائي. |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


يضبط ارتفاع الصف في نطاق مستطيل تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| endRow | int | فهرس الصف النهائي. |
| startColumn | int | فهرس العمود الابتدائي. |
| endColumn | int | فهرس العمود النهائي. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| onlyAuto | boolean | صحيح، يقوم بتعديل ارتفاع الصف تلقائيًا فقط عندما لا يكون ارتفاع الصف مخصصًا. |

### autoFitRows(AutoFitterOptions options) {#autoFitRows-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(AutoFitterOptions options)
```


يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | خيارات الضبط التلقائي. |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


يضبط ارتفاع الصف في نطاق تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| endRow | int | فهرس الصف النهائي. |

### autoFitRows(int startRow, int endRow, AutoFitterOptions options) {#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(int startRow, int endRow, AutoFitterOptions options)
```


يضبط ارتفاع الصف في نطاق تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| endRow | int | فهرس الصف النهائي. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | خيارات الضبط التلقائي. |

### calculateArrayFormula(String formula, CalculationOptions opts) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts)
```


يحسب صيغة كصيغة مصفوفة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة التي سيتم حسابها. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | خيارات حساب الصيغة |

**Returns:**
java.lang.Object[][]
### calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)
```


يحسب صيغة كصيغة مصفوفة.

**Remarks**

سيتم اعتبار الصيغة كصيغة مصفوفة ديناميكية لحساب الأبعاد والنتيجة. يُستخدم البُعد الأقصى المحدد من قبل المستخدم في الحالات التي تكون فيها النتيجة المحسوبة مجموعة بيانات كبيرة (على سبيل المثال، قد تتطابق النتيجة المحسوبة مع بيانات صف كامل أو عمود كامل) لكن المستخدم لا يحتاج إلى مصفوفة كبيرة بهذا الحجم وفقًا لمتطلبات العمل أو لأسباب الأداء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة التي سيتم حسابها. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | خيارات حساب الصيغة |
| maxRowCount | int | الحد الأقصى لعدد الصفوف للبيانات الناتجة. إذا كان غير موجب أو أكبر من عدد الصفوف الفعلي، فسيتم استخدام عدد الصفوف الفعلي. |
| maxColumnCount | int | الحد الأقصى لعدد الأعمدة للبيانات الناتجة. إذا كان غير موجب أو أكبر من عدد الأعمدة الفعلي، فسيتم استخدام عدد الأعمدة الفعلي. |

**Returns:**
java.lang.Object[][] - نتيجة الصيغة المحسوبة.
### calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData) {#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-}
```
public Object[][] calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)
```


يحسب صيغة كصيغة مصفوفة.

**Remarks**

سيتم اعتبار الصيغة كصيغة مصفوفة ديناميكية لحساب الأبعاد والنتيجة. يُستخدم البُعد الأقصى المحدد من قبل المستخدم في الحالات التي تكون فيها النتيجة المحسوبة مجموعة بيانات كبيرة (على سبيل المثال، قد تتطابق النتيجة المحسوبة مع بيانات صف كامل أو عمود كامل) لكن المستخدم لا يحتاج إلى مصفوفة كبيرة بهذا الحجم وفقًا لمتطلبات العمل أو لأسباب الأداء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة التي سيتم حسابها. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | خيارات حساب الصيغة |
| baseCellRow | int | فهرس الصف للخلية الأساسية. |
| baseCellColumn | int | فهرس العمود للخلية الأساسية. |
| maxRowCount | int | الحد الأقصى لعدد الصفوف للبيانات الناتجة. إذا كان غير موجب أو أكبر من عدد الصفوف الفعلي، فسيتم استخدام عدد الصفوف الفعلي. |
| maxColumnCount | int | الحد الأقصى لعدد الأعمدة للبيانات الناتجة. إذا كان غير موجب أو أكبر من عدد الصفوف الفعلي، فسيتم استخدام عدد الأعمدة الفعلي. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | بيانات الحساب. تُستخدم في الحالة التي يحتاج فيها المستخدم إلى حساب بعض الصيغ الثابتة عند تنفيذ محرك حساب مخصص. لهذا النوع من الحالات، يجب على المستخدم تحديدها باستخدام بيانات الحساب المقدمة لـ [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object[][] - نتيجة الصيغة المحسوبة.
### calculateFormula(CalculationOptions options, boolean recursive) {#calculateFormula-com.aspose.cells.CalculationOptions-boolean-}
```
public void calculateFormula(CalculationOptions options, boolean recursive)
```


يحسب جميع الصيغ في ورقة العمل هذه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | خيارات الحساب |
| recursive | boolean | True يعني إذا كانت خلايا ورقة العمل تعتمد على خلايا أوراق عمل أخرى، فسيتم حساب الخلايا التابعة في الأوراق الأخرى أيضًا. False يعني أنه تم حساب جميع الصيغ في ورقة العمل والقيم صحيحة. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


يحسب صيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة التي سيتم حسابها. |

**Returns:**
java.lang.Object - نتيجة الصيغة المحسوبة.
### calculateFormula(String formula, CalculationOptions opts) {#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object calculateFormula(String formula, CalculationOptions opts)
```


يحسب تعبير الصيغة مباشرة.

**Remarks**

سيتم حساب الصيغة كما لو تم تعيينها للخلية A1. وستُعامل الصيغة كصيغة عادية. إذا كنت بحاجة إلى حساب الصيغة كصيغة مصفوفة والحصول على مصفوفة للنتيجة المحسوبة، يرجى استخدام [calculateArrayFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-CalculationOptions-) بدلاً من ذلك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة التي سيتم حسابها. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | خيارات حساب الصيغة |

**Returns:**
java.lang.Object - النتيجة المحسوبة للصيغة المعطاة. قد يكون الكائن المرتجع من أحد الأنواع الممكنة لـ [Cell.getValue()](../../com.aspose.cells/cell\#getValue--)، أو ReferredArea.
### calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData) {#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-}
```
public Object calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)
```


يحسب تعبير الصيغة مباشرة.

**Remarks**

سيتم حساب الصيغة كما لو تم تعيينها للخلية الأساسية المحددة. وستُعامل الصيغة كصيغة عادية. إذا كنت بحاجة إلى حساب الصيغة كصيغة مصفوفة والحصول على مصفوفة للنتيجة المحسوبة، يرجى استخدام [calculateArrayFormula(String,FormulaParseOptions,CalculationOptions,int,int,int,int,CalculationData)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-FormulaParseOptions-CalculationOptions-int-int-int-int-CalculationData-) بدلاً من ذلك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة التي سيتم حسابها. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة. |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | خيارات حساب الصيغة. |
| baseCellRow | int | فهرس الصف للخلية الأساسية. |
| baseCellColumn | int | فهرس العمود للخلية الأساسية. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | بيانات الحساب. تُستخدم في الحالة التي يحتاج فيها المستخدم إلى حساب بعض الصيغ الثابتة عند تنفيذ محرك حساب مخصص. لهذا النوع من الحالات، يجب على المستخدم تحديدها باستخدام بيانات الحساب المقدمة لـ [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object - النتيجة المحسوبة للصيغة المعطاة. قد يكون الكائن المرتجع من أحد الأنواع الممكنة لـ [Cell.getValue()](../../com.aspose.cells/cell\#getValue--)، أو ReferredArea.
### clearComments() {#clearComments--}
```
public void clearComments()
```


يمسح جميع التعليقات في جدول البيانات المصمم.

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


يغلق الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات في ورقة العمل هذه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). خيارات الوصول إلى البيانات |

### convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn) {#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-}
```
public String convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)
```


يحول نمط مرجع الصيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة المراد تحويلها. |
| toR1C1 | boolean | أي نمط إشارة لتحويل الصيغة إليه. إذا كانت الصيغة الأصلية بنمط الإشارة A1، يجب أن تكون هذه القيمة true حتى يتم تحويل الصيغة من A1 إلى نمط الإشارة R1C1؛ إذا كانت الصيغة الأصلية بنمط الإشارة R1C1، يجب أن تكون هذه القيمة false حتى يتم تحويل الصيغة من R1C1 إلى نمط الإشارة A1؛ |
| baseCellRow | int | فهرس الصف للخلية الأساسية. |
| baseCellColumn | int | فهرس العمود للخلية الأساسية. |

**Returns:**
java.lang.String - الصيغة المحوّلة.
### copy(Worksheet sourceSheet) {#copy-com.aspose.cells.Worksheet-}
```
public void copy(Worksheet sourceSheet)
```


ينسخ المحتويات والتنسيقات من ورقة عمل أخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | ورقة العمل المصدر. |

### copy(Worksheet sourceSheet, CopyOptions copyOptions) {#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-}
```
public void copy(Worksheet sourceSheet, CopyOptions copyOptions)
```


ينسخ المحتويات والتنسيقات من ورقة عمل أخرى.

**Remarks**

يمكنك نسخ البيانات من ورقة عمل أخرى في نفس الملف أو ملف آخر. ومع ذلك، لا يدعم هذا الأسلوب نسخ كائنات الرسم، مثل التعليقات والصور والمخططات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | ورقة العمل المصدر. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

### dispose() {#dispose--}
```
public void dispose()
```


ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### filter(CellArea ca) {#filter-com.aspose.cells.CellArea-}
```
public void filter(CellArea ca)
```


يقوم بتصفية النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


يثبت الألواح عند الخلية المحددة في ورقة العمل.

**Remarks**

لا يمكن أن يكون كل من فهرس الصف وفهرس العمود صفرًا. كما لا يمكن أن يكون عدد الصفوف وعدد الأعمدة صفرًا.

المعاملان الأولان يحددان موضع التجمد، والمعاملان الأخيران يحددان المنطقة المجمدة في الجزء العلوي الأيسر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| عمود | int | فهرس العمود. |
| freezedRows | int | عدد الصفوف المرئية في الجزء العلوي، لا يزيد عن فهرس الصف. |
| freezedColumns | int | عدد الأعمدة المرئية في الجزء الأيسر، لا يزيد عن فهرس العمود. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


يثبت الألواح عند الخلية المحددة في ورقة العمل.

**Remarks**

لا يمكن أن يكون كل من فهرس الصف وفهرس العمود صفرًا. كما لا يمكن أن يكون عدد الصفوف وعدد الأعمدة صفرًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |
| freezedRows | int | عدد الصفوف المرئية في الجزء العلوي، لا يزيد عن فهرس الصف. |
| freezedColumns | int | عدد الأعمدة المرئية في الجزء الأيسر، لا يزيد عن فهرس العمود. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


يحصل على الخلية النشطة في ورقة العمل.

**Returns:**
java.lang.String
### getAdvancedFilter() {#getAdvancedFilter--}
```
public AdvancedFilter getAdvancedFilter()
```


يحصل على إعدادات الفلتر المتقدم.

**Returns:**
[AdvancedFilter](../../com.aspose.cells/advancedfilter) - 
### getAllPictures() {#getAllPictures--}
```
public Picture[] getAllPictures()
```


يحصل على جميع الصور بما في ذلك الصور المدمجة في الخلية وفوق الخلايا.

**Returns:**
com.aspose.cells.Picture[] -
### getAllowEditRanges() {#getAllowEditRanges--}
```
public ProtectedRangeCollection getAllowEditRanges()
```


يحصل على مجموعة نطاقات السماح بالتعديل في ورقة العمل.

**Returns:**
[ProtectedRangeCollection](../../com.aspose.cells/protectedrangecollection)
### getAreasOfXmlMapQuery(String path, XmlMap xmlMap) {#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public CellArea[] getAreasOfXmlMapQuery(String path, XmlMap xmlMap)
```


يستعلم عن مناطق الخلايا التي تم ربطها/ربطها بالمسار المحدد لخريطة XML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | java.lang.String | مسار عنصر xml |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | حدد خريطة xml إذا كنت تريد الاستعلام عن المسار المحدد داخل خريطة معينة |

**Returns:**
com.aspose.cells.CellArea[] - قائمة [CellArea](../../com.aspose.cells/cellarea) التي تم ربطها/تعيينها إلى المسار المحدد لخريطة xml، يتم إرجاع قائمة فارغة إذا لم يتم ربط/تعيين أي شيء.
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


يمثل الفلتر التلقائي لورقة العمل المحددة.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


يحصل على صورة خلفية ورقة العمل.

**Returns:**
byte[]
### getCellWatches() {#getCellWatches--}
```
public CellWatchCollection getCellWatches()
```


يحصل على مجموعة الخلايا في هذه ورقة العمل التي يتم مراقبتها في 'نافذة المراقبة'.

**Returns:**
[CellWatchCollection](../../com.aspose.cells/cellwatchcollection)
### getCells() {#getCells--}
```
public Cells getCells()
```


يحصل على مجموعة [Cells](../../com.aspose.cells/cells).

**Returns:**
[Cells](../../com.aspose.cells/cells)
### getCharts() {#getCharts--}
```
public ChartCollection getCharts()
```


يحصل على مجموعة [Chart](../../com.aspose.cells/chart)

**Returns:**
[ChartCollection](../../com.aspose.cells/chartcollection)
### getCheckBoxes() {#getCheckBoxes--}
```
public CheckBoxCollection getCheckBoxes()
```


يحصل على مجموعة [CheckBox](../../com.aspose.cells/checkbox).

**Returns:**
[CheckBoxCollection](../../com.aspose.cells/checkboxcollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


يحصل على اسم رمز ورقة العمل.

**Returns:**
java.lang.String
### getComments() {#getComments--}
```
public CommentCollection getComments()
```


يحصل على مجموعة [Comment](../../com.aspose.cells/comment).

**Returns:**
[CommentCollection](../../com.aspose.cells/commentcollection)
### getConditionalFormattings() {#getConditionalFormattings--}
```
public ConditionalFormattingCollection getConditionalFormattings()
```


يحصل على ConditionalFormattings في ورقة العمل.

**Returns:**
[ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection)
### getCustomProperties() {#getCustomProperties--}
```
public CustomPropertyCollection getCustomProperties()
```


يحصل على كائن يمثل معلومات المعرف المرتبطة بورقة عمل.

**Remarks**

توفر Worksheet.CustomProperties آلية مفضلة لتخزين البيانات العشوائية. تدعم مكونات المستندات التابعة لجهات خارجية القديمة، وكذلك الحالات التي تتطلب أجزاءً ثنائيةً بشكل صارم.

**Returns:**
[CustomPropertyCollection](../../com.aspose.cells/custompropertycollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


يشير إلى ما إذا كان ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. القيمة الافتراضية هي false.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


صحيح إذا تم عرض القيم الصفرية.

**Returns:**
boolean
### getErrorCheckOptions() {#getErrorCheckOptions--}
```
public ErrorCheckOptionCollection getErrorCheckOptions()
```


يحصل على إعداد فحص الأخطاء المطبق على نطاقات معينة.

**Returns:**
[ErrorCheckOptionCollection](../../com.aspose.cells/errorcheckoptioncollection)
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


يمثل فهرس العمود الأول الظاهر.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


يمثل فهرس الصف الأول الظاهر.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


يحصل على تجميد الألواح.

**Returns:**
int[] - إرجاع null يعني أن ورقة العمل غير مُجمدة 0:فهرس الصف;1:العمود;2:الصفوف المجمدة;3:الصفوف المجمدة
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


يحصل على لون خط الشبكة

**Returns:**
[Color](../../com.aspose.cells/color)
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public HorizontalPageBreakCollection getHorizontalPageBreaks()
```


يحصل على مجموعة [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection).

**Returns:**
[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)
### getHyperlinks() {#getHyperlinks--}
```
public HyperlinkCollection getHyperlinks()
```


يحصل على مجموعة [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection).

**Returns:**
[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


يحصل على فهرس الورقة في مجموعة أوراق العمل.

**Returns:**
int
### getListObjects() {#getListObjects--}
```
public ListObjectCollection getListObjects()
```


يحصل على جميع ListObjects في هذه ورقة العمل.

**Returns:**
[ListObjectCollection](../../com.aspose.cells/listobjectcollection)
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم ورقة العمل.

**Remarks**

الحد الأقصى لطول اسم الورقة هو 31. ولا يمكنك تعيين نفس الاسم (بدون حساسية لحالة الأحرف) لورقتين عمل. على سبيل المثال، لا يمكنك تعيين "SheetName1" للورقة الأولى وتعيين "SHEETNAME1" للورقة الثانية.

**Returns:**
java.lang.String
### getOleObjects() {#getOleObjects--}
```
public OleObjectCollection getOleObjects()
```


يمثل مجموعة من [OleObject](../../com.aspose.cells/oleobject) في ورقة عمل.

**Returns:**
[OleObjectCollection](../../com.aspose.cells/oleobjectcollection)
### getOutline() {#getOutline--}
```
public Outline getOutline()
```


يحصل على المخطط التفصيلي في هذه ورقة العمل.

**Returns:**
[Outline](../../com.aspose.cells/outline)
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


يمثل وصف إعداد الصفحة في هذه الورقة.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPaneState() {#getPaneState--}
```
public int getPaneState()
```


يشير إلى ما إذا كان الجزء يحتوي على تقسيمات أفقية أو عمودية، وما إذا كانت تلك التقسيمات مجمدة.

انظر [PaneStateType](../../com.aspose.cells/panestatetype).

**Returns:**
int
### getPanes() {#getPanes--}
```
public PaneCollection getPanes()
```


يحصل على أجزاء النافذة.

**Remarks**

إذا لم يتم تقسيم النافذة أو تجميدها.

**Returns:**
[PaneCollection](../../com.aspose.cells/panecollection)
### getPictures() {#getPictures--}
```
public PictureCollection getPictures()
```


يحصل على مجموعة [Picture](../../com.aspose.cells/picture).

**Returns:**
[PictureCollection](../../com.aspose.cells/picturecollection)
### getPivotTables() {#getPivotTables--}
```
public PivotTableCollection getPivotTables()
```


يحصل على جميع جداول المحور في هذه ورقة العمل.

**Returns:**
[PivotTableCollection](../../com.aspose.cells/pivottablecollection)
### getPrintingPageBreaks(ImageOrPrintOptions options) {#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-}
```
public CellArea[] getPrintingPageBreaks(ImageOrPrintOptions options)
```


يحصل على فواصل الصفحات التلقائية.

**Remarks**

كل مساحة خلية تمثل ورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | خيارات الطباعة |

**Returns:**
com.aspose.cells.CellArea[] - مناطق فواصل الصفحات التلقائية.
### getProtection() {#getProtection--}
```
public Protection getProtection()
```


يمثل الأنواع المختلفة لخيارات الحماية المتاحة لورقة العمل. يدعم خيارات الحماية المتقدمة في ExcelXP والإصدارات الأحدث.

**Remarks**

يمكن لهذه الخاصية حماية ورقة العمل في جميع إصدارات ملف Excel وتدعم خيارات الحماية المتقدمة في ExcelXP والإصدارات الأحدث.

**Returns:**
[Protection](../../com.aspose.cells/protection)
### getQueryTables() {#getQueryTables--}
```
public QueryTableCollection getQueryTables()
```


يحصل على [QueryTableCollection](../../com.aspose.cells/querytablecollection) في ورقة العمل.

**Returns:**
[QueryTableCollection](../../com.aspose.cells/querytablecollection)
### getScenarios() {#getScenarios--}
```
public ScenarioCollection getScenarios()
```


يحصل على مجموعة [Scenario](../../com.aspose.cells/scenario).

**Returns:**
[ScenarioCollection](../../com.aspose.cells/scenariocollection)
### getSelectedAreas() {#getSelectedAreas--}
```
public Range[] getSelectedAreas()
```


يحصل على النطاقات المحددة من الخلايا في جدول البيانات المصمم.

**Returns:**
com.aspose.cells.Range[] - إرجاع جميع النطاقات المحددة.
### getSelectedRanges() {#getSelectedRanges--}
```
public ArrayList getSelectedRanges()
```


يحصل على النطاقات المحددة من الخلايا في جدول البيانات المصمم.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Worksheet.GetSelectedAreas(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.util.ArrayList - قائمة ArrayList التي تحتوي على النطاقات المحددة.
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


يعيد جميع أشكال الرسم في هذه ورقة العمل.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTypeIcons() {#getShowDataTypeIcons--}
```
public boolean getShowDataTypeIcons()
```


يشير إلى ما إذا كان يجب إظهار أيقونات نوع البيانات.

**Returns:**
boolean
### getShowFormulas() {#getShowFormulas--}
```
public boolean getShowFormulas()
```


يشير إلى ما إذا كان يجب إظهار الصيغ أو نتائجها.

**Returns:**
boolean
### getSlicers() {#getSlicers--}
```
public SlicerCollection getSlicers()
```


احصل على مجموعة Slicer في ورقة العمل

**Returns:**
[SlicerCollection](../../com.aspose.cells/slicercollection)
### getSmartTagSetting() {#getSmartTagSetting--}
```
public SmartTagSetting getSmartTagSetting()
```


يحصل على جميع كائنات [SmartTagCollection](../../com.aspose.cells/smarttagcollection) في ورقة العمل.

**Returns:**
[SmartTagSetting](../../com.aspose.cells/smarttagsetting)
### getSparklineGroups() {#getSparklineGroups--}
```
public SparklineGroupCollection getSparklineGroups()
```


يحصل على مجموعات sparkline في ورقة العمل.

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


يمثل لون تبويب ورقة العمل.

**Remarks**

هذه الميزة مدعومة فقط في ExcelXP (Excel2002) والإصدارات اللاحقة. إذا حفظت الملف بصيغة Excel97 أو Excel2000، سيتم حذفها.

**Returns:**
[Color](../../com.aspose.cells/color)
### getTabId() {#getTabId--}
```
public int getTabId()
```


يحدد المعرف الداخلي للورقة.

**Returns:**
int
### getTextBoxes() {#getTextBoxes--}
```
public TextBoxCollection getTextBoxes()
```


يحصل على مجموعة [TextBox](../../com.aspose.cells/textbox).

**Returns:**
[TextBoxCollection](../../com.aspose.cells/textboxcollection)
### getTimelines() {#getTimelines--}
```
public TimelineCollection getTimelines()
```


احصل على مجموعة Timeline في ورقة العمل

**Returns:**
[TimelineCollection](../../com.aspose.cells/timelinecollection)
### getTransitionEntry() {#getTransitionEntry--}
```
public boolean getTransitionEntry()
```


يشير إلى ما إذا كان خيار إدخال صيغة الانتقال (توافق Lotus) مفعلاً.

**Returns:**
boolean
### getTransitionEvaluation() {#getTransitionEvaluation--}
```
public boolean getTransitionEvaluation()
```


يشير إلى ما إذا كان خيار تقييم صيغة الانتقال (توافق Lotus) مفعلاً.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


يمثل نوع ورقة العمل.

انظر [SheetType](../../com.aspose.cells/sheettype).

**Returns:**
int
### getUniqueId() {#getUniqueId--}
```
public String getUniqueId()
```


يحصل على المعرف الفريد، وهو نفسه \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public ValidationCollection getValidations()
```


يحصل على مجموعة إعدادات التحقق من صحة البيانات في ورقة العمل.

**Returns:**
[ValidationCollection](../../com.aspose.cells/validationcollection)
### getVerticalPageBreaks() {#getVerticalPageBreaks--}
```
public VerticalPageBreakCollection getVerticalPageBreaks()
```


يحصل على مجموعة [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection).

**Returns:**
[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)
### getViewType() {#getViewType--}
```
public int getViewType()
```


يحصل على نوع العرض.

انظر [ViewType](../../com.aspose.cells/viewtype).

**Returns:**
int
### getVisibilityType() {#getVisibilityType--}
```
public int getVisibilityType()
```


يشير إلى الحالة المرئية لهذه الورقة.

انظر [VisibilityType](../../com.aspose.cells/visibilitytype).

**Returns:**
int
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


يحصل على كائن المصنف الذي يحتوي على هذه الورقة.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


يمثل معامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400.

**Remarks**

يرجى ضبط نوع العرض أولاً.

**Returns:**
int
### hasAutofilter() {#hasAutofilter--}
```
public boolean hasAutofilter()
```


يشير إلى ما إذا كانت هذه ورقة العمل تحتوي على مرشح تلقائي.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


يحصل على قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true.

**Returns:**
boolean
### isOutlineShown() {#isOutlineShown--}
```
public boolean isOutlineShown()
```


يشير إلى ما إذا كان يجب إظهار المخطط.

**Returns:**
boolean
### isPageBreakPreview() {#isPageBreakPreview--}
```
public boolean isPageBreakPreview()
```


يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض في العرض العادي أو معاينة فواصل الصفحات.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


يشير إلى ما إذا كانت ورقة العمل محمية.

**Returns:**
boolean
### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}
```
public boolean isRowColumnHeadersVisible()
```


يحصل على قيمة تشير إلى ما إذا كانت ورقة العمل ستعرض رؤوس الصفوف والأعمدة. القيمة الافتراضية هي true.

**Returns:**
boolean
### isRulerVisible() {#isRulerVisible--}
```
public boolean isRulerVisible()
```


يشير إلى ما إذا كان المسطرة مرئية. يتم تطبيق هذه الخاصية فقط في معاينة فواصل الصفحات.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


يشير إلى ما إذا كانت ورقة العمل هذه مختارة عند فتح دفتر العمل.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


يمثل ما إذا كانت ورقة العمل مرئية.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


ينقل الورقة إلى موقع آخر في جدول البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الورقة الوجهة. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### protect(int type) {#protect-int-}
```
public void protect(int type)
```


يحمي ورقة العمل.

**Remarks**

تحمي هذه الطريقة ورقة العمل بدون كلمة مرور. يمكنها حماية ورقة العمل في جميع إصدارات ملف Excel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). نوع الحماية. |

### protect(int type, String password, String oldPassword) {#protect-int-java.lang.String-java.lang.String-}
```
public void protect(int type, String password, String oldPassword)
```


يحمي ورقة العمل.

**Remarks**

يمكن لهذه الطريقة حماية ورقة العمل في جميع إصدارات ملف Excel.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = excel.getWorksheets().get(0);
         //Protecting the worksheet with a password
         worksheet.protect(ProtectionType.ALL, "aspose", null);
         //Saving the modified Excel file in default (that is Excel 20003) format
         excel.save("output.xls");
         //Closing the file stream to free all resources
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). نوع الحماية. |
| password | java.lang.String | كلمة المرور. |
| oldPassword | java.lang.String | إذا كانت ورقة العمل محمية بالفعل بكلمة مرور، يرجى تقديم كلمة المرور القديمة. وإلا، يمكنك تعيين قيمة فارغة أو سلسلة نصية خالية لهذا المعامل. |

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


يقوم بتحديث جميع جداول PivotTables في هذه ورقة العمل.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


يقوم بتحديث جميع جداول PivotTables في هذه ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | الخيار لتحديث مصدر البيانات لجدول المحور. |

**Returns:**
boolean
### removeAllDrawingObjects() {#removeAllDrawingObjects--}
```
public void removeAllDrawingObjects()
```


يزيل جميع كائنات الرسم في هذه ورقة العمل.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


يزيل المرشح التلقائي لورقة العمل.

### removeSplit() {#removeSplit--}
```
public void removeSplit()
```


يزيل تقسيم النافذة.

### replace(String oldString, String newString) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String oldString, String newString)
```


يستبدل نص جميع الخلايا بسلسلة جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| oldString | java.lang.String | قيمة السلسلة القديمة. |
| newString | java.lang.String | قيمة السلسلة الجديدة. |

**Returns:**
int
### selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers) {#selectRange-int-int-int-int-boolean-}
```
public void selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)
```


يحدد نطاقًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | صف البداية. |
| startColumn | int | عمود البداية |
| totalRows | int | عدد الصفوف. |
| totalColumns | int | عدد الأعمدة |
| removeOthers | boolean | True يعني إزالة النطاقات المحددة الأخرى واختيار هذا النطاق فقط. |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


يضبط الخلية النشطة في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


يضبط صورة خلفية ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

### setCodeName(String value) {#setCodeName-java.lang.String-}
```
public void setCodeName(String value)
```


يحصل على اسم رمز ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


يشير إلى ما إذا كان ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


صحيح إذا تم عرض القيم الصفرية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


يمثل فهرس العمود الأول الظاهر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


يمثل فهرس الصف الأول الظاهر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


يضبط لون خط الشبكة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم ورقة العمل.

**Remarks**

الحد الأقصى لطول اسم الورقة هو 31. ولا يمكنك تعيين نفس الاسم (بدون حساسية لحالة الأحرف) لورقتين عمل. على سبيل المثال، لا يمكنك تعيين "SheetName1" للورقة الأولى وتعيين "SHEETNAME1" للورقة الثانية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


يشير إلى ما إذا كان يجب إظهار المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPageBreakPreview(boolean value) {#setPageBreakPreview-boolean-}
```
public void setPageBreakPreview(boolean value)
```


يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض في العرض العادي أو معاينة فواصل الصفحات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRowColumnHeadersVisible(boolean value) {#setRowColumnHeadersVisible-boolean-}
```
public void setRowColumnHeadersVisible(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت ورقة العمل ستعرض رؤوس الصفوف والأعمدة. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRulerVisible(boolean value) {#setRulerVisible-boolean-}
```
public void setRulerVisible(boolean value)
```


يشير إلى ما إذا كان المسطرة مرئية. يتم تطبيق هذه الخاصية فقط في معاينة فواصل الصفحات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


يشير إلى ما إذا كانت ورقة العمل هذه مختارة عند فتح دفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowDataTypeIcons(boolean value) {#setShowDataTypeIcons-boolean-}
```
public void setShowDataTypeIcons(boolean value)
```


يشير إلى ما إذا كان يجب إظهار أيقونات نوع البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowFormulas(boolean value) {#setShowFormulas-boolean-}
```
public void setShowFormulas(boolean value)
```


يشير إلى ما إذا كان يجب إظهار الصيغ أو نتائجها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.cells.Color-}
```
public void setTabColor(Color value)
```


يمثل لون تبويب ورقة العمل.

**Remarks**

هذه الميزة مدعومة فقط في ExcelXP (Excel2002) والإصدارات اللاحقة. إذا حفظت الملف بصيغة Excel97 أو Excel2000، سيتم حذفها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setTabId(int value) {#setTabId-int-}
```
public void setTabId(int value)
```


يحدد المعرف الداخلي للورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTransitionEntry(boolean value) {#setTransitionEntry-boolean-}
```
public void setTransitionEntry(boolean value)
```


يشير إلى ما إذا كان خيار إدخال صيغة الانتقال (توافق Lotus) مفعلاً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTransitionEvaluation(boolean value) {#setTransitionEvaluation-boolean-}
```
public void setTransitionEvaluation(boolean value)
```


يشير إلى ما إذا كان خيار تقييم صيغة الانتقال (توافق Lotus) مفعلاً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يمثل نوع ورقة العمل.

انظر [SheetType](../../com.aspose.cells/sheettype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setUniqueId(String value) {#setUniqueId-java.lang.String-}
```
public void setUniqueId(String value)
```


يضبط المعرف الفريد، وهو نفسه \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setViewType(int value) {#setViewType-int-}
```
public void setViewType(int value)
```


يضبط نوع العرض.

انظر [ViewType](../../com.aspose.cells/viewtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setVisibilityType(int value) {#setVisibilityType-int-}
```
public void setVisibilityType(int value)
```


يشير إلى الحالة المرئية لهذه الورقة.

انظر [VisibilityType](../../com.aspose.cells/visibilitytype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يمثل ما إذا كانت ورقة العمل مرئية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setVisible(boolean isVisible, boolean ignoreError) {#setVisible-boolean-boolean-}
```
public void setVisible(boolean isVisible, boolean ignoreError)
```


يضبط الخيارات المرئية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isVisible | boolean | ما إذا كانت ورقة العمل مرئية |
| ignoreError | boolean | ما إذا كان يجب تجاهل الخطأ إذا كان هذا الخيار غير صالح. |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


يمثل معامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400.

**Remarks**

يرجى ضبط نوع العرض أولاً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### split() {#split--}
```
public void split()
```


يقسم النافذة.

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


يبدأ الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات في ورقة العمل هذه.

**Remarks**

بعد الانتهاء من الوصول إلى البيانات، يجب استدعاء [closeAccessCache(int)](../../com.aspose.cells/worksheet\#closeAccessCache-int-) بنفس الخيارات لمسح جميع الذاكرات المؤقتة واستعادة وضع الوصول العادي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). خيارات الوصول إلى البيانات |

### toString() {#toString--}
```
public String toString()
```


يرجع سلسلة تمثل كائن ورقة العمل الحالي.

**Returns:**
java.lang.String -
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


يفك تجميد الألواح في ورقة العمل.

### unprotect() {#unprotect--}
```
public void unprotect()
```


يلغي حماية ورقة العمل.

**Remarks**

هذه الطريقة تزيل حماية ورقة العمل التي تم حمايتها بدون كلمة مرور.

### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


يلغي حماية ورقة العمل.

**Remarks**

إذا كانت ورقة العمل محمية بدون كلمة مرور، يمكنك تعيين قيمة فارغة (null) أو سلسلة نصية فارغة إلى معلمة كلمة المرور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| password | java.lang.String | كلمة المرور |

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### xmlMapQuery(String path, XmlMap xmlMap) {#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public ArrayList xmlMapQuery(String path, XmlMap xmlMap)
```


يستعلم عن مناطق الخلايا التي تم ربطها/ربطها بالمسار المحدد لخريطة XML.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Worksheet.GetAreasOfXmlMapQuery(). سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | java.lang.String | مسار عنصر xml |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | حدد خريطة xml إذا كنت تريد الاستعلام عن المسار المحدد داخل خريطة معينة |

**Returns:**
java.util.ArrayList - قائمة [CellArea](../../com.aspose.cells/cellarea) التي تم ربطها/تعيينها إلى المسار المحدد لخريطة XML، تُرجع قائمة فارغة إذا لم يتم ربط/تعيين أي شيء.
