---
title: "MainWeb"
second_title: "Aspose.Cells for Java API Reference"
description: "الفئة الأصلية لعنصر تحكم GridWeb. للاستخدام الداخلي فقط."
type: docs
url: /ar/java/com.aspose.gridweb/mainweb/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebControl](../../com.aspose.gridweb/webcontrol), [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol)
```
public class MainWeb extends ExtWebControl
```

الفئة الأصلية لعنصر تحكم GridWeb. للاستخدام الداخلي فقط.

**Example**

```
         		GridWeb GridWeb1 = new GridWeb();
         //do your business
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [MainWeb()](#MainWeb--) | البناء الافتراضي لـ control MainWeb. |
## حقول

| حقل | الوصف |
| --- | --- |
| [AfterColumnFilter](#AfterColumnFilter) | يحدث بعد تصفية العمود. |
| [AjaxCallFinished](#AjaxCallFinished) | يتم إطلاقه عندما ينتهي تحديث الـ ajax للعنصر. |
| [BeforeColumnFilter](#BeforeColumnFilter) | يحدث قبل تصفية العمود. |
| [CellClickOnAjax](#CellClickOnAjax) | يحدث عندما يتم النقر على الخلية، ويحتاج إلى إجراء ajaxcallback لهذا الحدث. |
| [CellClientUpdate](#CellClientUpdate) | يحدث عندما يحدث تحديث خلية من جانب العميل. |
| [CellCommand](#CellCommand) | يحدث عندما يتم النقر على ارتباط الأمر الخاص بالخلية. |
| [CellDoubleClick](#CellDoubleClick) | يحدث عندما يتم النقر المزدوج على الخلية. |
| [CellModifiedOnAjax](#CellModifiedOnAjax) | يحدث عندما يتم تعديل الخلية في ajaxcall. |
| [ColumnDeleted](#ColumnDeleted) | يحدث عندما يحذف المستخدم عمودًا من القائمة الجانبية للعميل. |
| [ColumnDeleting](#ColumnDeleting) | يحدث عندما يحاول المستخدم حذف عمود من القائمة الجانبية للعميل. |
| [ColumnDoubleClick](#ColumnDoubleClick) | يحدث عندما يتم النقر المزدوج على رأس العمود. |
| [ColumnInserted](#ColumnInserted) | يحدث عندما يُدخل المستخدم عمودًا من القائمة الجانبية للعميل. |
| [CustomCommand](#CustomCommand) | يحدث عندما ينقر المستخدم على زر أمر مخصص. |
| [LoadCustomData](#LoadCustomData) | يتم إطلاقه عندما يتم تعيين SessionMode الخاص بالتحكم إلى Custom ويحتاج إلى تحميل بيانات الورقة. |
| [PageIndexChanged](#PageIndexChanged) | يحدث عندما يتغير فهرس صفحة الورقة في التحكم. |
| [RowDeleted](#RowDeleted) | يحدث عندما يقوم المستخدم بحذف صف من القائمة الجانبية للعميل. |
| [RowDeleting](#RowDeleting) | يحدث عندما يحاول المستخدم حذف صف من القائمة الجانبية للعميل. |
| [RowDoubleClick](#RowDoubleClick) | يحدث عندما يتم النقر المزدوج على رأس الصف. |
| [RowInserted](#RowInserted) | يحدث عندما يقوم المستخدم بإدراج صف من القائمة الجانبية للعميل. |
| [SaveCommand](#SaveCommand) | يحدث عندما يتم النقر على زر "save". |
| [SheetAdded](#SheetAdded) | يحدث عندما يضيف المستخدم ورقة عمل من قائمة شريط الأدوات. |
| [SheetTabClick](#SheetTabClick) | يحدث عندما يتم النقر على تبويب الورقة. |
| [SubmitCommand](#SubmitCommand) | يحدث عندما يتم النقر على زر "submit". |
| [UndoCommand](#UndoCommand) | يحدث عندما يتم النقر على زر "undo". |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | يحسب نتيجة الصيغ. |
| [createChildControls()](#createChildControls--) | تنفيذ CreateChildControls من WebControl، يستخدم داخليًا فقط. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | يحصل على مسار الويب لملفات السكريبت/الصورة الخاصة بالتحكم. |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | يحصل على عنوان URL الويب لملف اللغة الخاص بالتحكم. |
| [getActiveCell()](#getActiveCell--) | يحصل على الخلية النشطة في الورقة الحالية. |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | يحدد لون الخلفية للخلية النشطة. |
| [getActiveCellColor()](#getActiveCellColor--) | يحدد لون الخلية النشطة. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | يحدد لون الخلفية لرأس الصف/العمود النشط. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | يحدد لون رأس الصف/العمود النشط. |
| [getActiveSheet()](#getActiveSheet--) | يحصل على الورقة النشطة |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | يحصل على فهرس الورقة النشطة. |
| [getActiveTabStyle()](#getActiveTabStyle--) | يحدد نمط التبويب النشط. |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | يحصل على ما إذا كانت صورة Chart يتم تحديثها أثناء تحديث قيمة الخلية. القيمة الافتراضية هي true |
| [getBackColor()](#getBackColor--) | يحصل على BackColor في WebControl |
| [getBorderColor()](#getBorderColor--) | يحصل على BorderColor في WebControl |
| [getBorderStyle()](#getBorderStyle--) | يحصل على BorderStyle في WebControl |
| [getBorderWidth()](#getBorderWidth--) | يحصل على BorderWidth في WebControl |
| [getBottomTableStyle()](#getBottomTableStyle--) | يحصل على نمط الشريط السفلي للتحكم. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | يحصل على CssClass في WebControl |
| [getCurrentPageIndex()](#getCurrentPageIndex--) | يحصل على فهرس الصفحة الحالية في وضع التصفح. |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | يمثل محرك حساب مخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells. |
| [getCustomCommandButtons()](#getCustomCommandButtons--) | يحصل على مجموعة أزرار الأوامر المخصصة |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | يحصل على اسم ملف النمط المخصص. |
| [getDPI()](#getDPI--) | يحصل على / يضبط DPI للجهاز. |
| [getDefaultFontName()](#getDefaultFontName--) | يحصل على اسم الخط الافتراضي للعنصر. |
| [getDefaultFontSize()](#getDefaultFontSize--) | يحصل على حجم الخط الافتراضي للعنصر. |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | يحصل على لون خط الشبكة الافتراضي. |
| [getDisplayCellTip()](#getDisplayCellTip--) | يحصل على ما إذا كان سيتم إظهار التلميحات. القيمة الافتراضية هي true. |
| [getEditMode()](#getEditMode--) | يحصل على وضع التحرير للعنصر. |
| [getEnableAJAX()](#getEnableAJAX--) | يحصل على ما إذا كان سيتم استخدام استدعاء AJAX. القيمة الافتراضية هي true. |
| [getEnableAsync()](#getEnableAsync--) | يحصل على ما إذا كان سيتم تحميل بيانات الخلايا بطريقة غير متزامنة، يُنصح بتطبيق ذلك على ورقة واحدة تحتوي على أكثر من 10000 خلية. |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | يحصل على ما إذا كان سيتم تمكين عمليات الأعمدة على جانب العميل. |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | يحصل على ما إذا كان سيتم تمكين عمليات التجميد على جانب العميل. |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | يحصل على ما إذا كان سيتم تمكين عمليات الدمج على جانب العميل. |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | يحصل على ما إذا كان سيتم تمكين تغيير حجم الأعمدة والصفوف على جانب العميل. |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | يحصل على ما إذا كان سيتم تمكين عمليات الصفوف على جانب العميل. |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | يحصل على ما إذا كان سيتم تمكين حدث النقر المزدوج على جانب العميل. |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | يحصل على ما إذا كان سيتم تطبيق تأثير الضوء المعدني. |
| [getEnablePaging()](#getEnablePaging--) | يحصل على ما إذا كان سيتم تمكين وضع الصفحات للعنصر. |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | يحصل على ما إذا كان سيتم تمكين مربع حوار النمط على جانب العميل. |
| [getEnabled()](#getEnabled--) | يحصل على Enabled في WebControl |
| [getFilteredPaging()](#getFilteredPaging--) | يحصل على ما إذا كان سيتم تمكين الصفحات بعد تصفية البيانات، سيصبح ساريًا عندما تكون EnablePaging true. |
| [getFont()](#getFont--) | يحصل على Font في WebControl |
| [getForceValidation()](#getForceValidation--) | يحصل على ما إذا كان سيتم فرض التحقق على جانب العميل. |
| [getForeColor()](#getForeColor--) | يحصل على ForeColor في WebControl |
| [getFrameTableStyle()](#getFrameTableStyle--) | يحصل على نمط الإطار للعنصر. |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | يحصل على ما إذا كان GridWeb سيقوم بعملية الحفظ الافتراضية، القيمة الافتراضية هي true. |
| [getHeaderBarHeight()](#getHeaderBarHeight--) | يحصل على ارتفاع (System.Web.UI.WebControl.Unit) شريط الرأس العلوي للعنصر. |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | يحصل على نمط شريط الرأس. |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | يحصل على نمط شريط الرأس للعنصر |
| [getHeaderBarWidth()](#getHeaderBarWidth--) | يحصل على عرض ( System.Web.UI.WebControl.Unit ) أو شريط الرأس الأيسر للعنصر. |
| [getHeight()](#getHeight--) | يحصل على ارتفاع ( System.Web.UI.WebControl.Unit ) للعنصر. |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | يحصل على ما إذا كان GridWeb يتجاهل إظهار الصفوف أو الأعمدة التي لا تحتوي على قيم خلايا ولكنها لا تزال مُنسقة. |
| [getLoadOptions()](#getLoadOptions--) | يمثل خيارات التحميل لـ GridWeb. |
| [getMaxColumn()](#getMaxColumn--) | يحصل على أقصى فهرس عمود للعرض (مبني على الصفر) للورقة الويب. |
| [getMaxRow()](#getMaxRow--) | يحصل على أقصى فهرس صف للعرض (مبني على الصفر) للورقة الويب. |
| [getMessage()](#getMessage--) | يحصل على الرسالة الخاصة بالشبكة. |
| [getMinColumn()](#getMinColumn--) | يحصل على أدنى فهرس عمود للعرض (مبني على الصفر) للورقة الويب. |
| [getMinRow()](#getMinRow--) | يحصل على أدنى فهرس صف للعرض (مبني على الصفر) للورقة الويب. |
| [getModifiedCells()](#getModifiedCells--) | يحصل على مجموعة الخلايا التي تم تعديلها من قبل العميل. |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | يحصل على ما إذا كان يجب إظهار صفوف المجموعات. |
| [getNoHScroll()](#getNoHScroll--) | يحصل على قيمة تشير إلى ما إذا كان شريط التمرير الأفقي مخفيًا. |
| [getNoScroll()](#getNoScroll--) | يحصل على ما إذا كان يجب إظهار شريط التمرير. |
| [getNoVScroll()](#getNoVScroll--) | يحصل على قيمة تشير إلى ما إذا كان شريط التمرير العمودي مخفيًا. |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | يحصل على اسم الدالة من جانب العميل التي تُستدعى عند انتهاء ajaxcall. |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | يحصل على اسم الدالة من جانب العميل التي تُستدعى عندما تفشل عملية التحقق من صحة الخلية. |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | يحصل على الدالة من جانب العميل التي تُستدعى عند تحديد خلية. |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | يحصل على الدالة من جانب العميل التي تُستدعى عند تحديد خلية. |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | يحصل على الدالة من جانب العميل التي تُستدعى عند إلغاء تحديد خلية. |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | يحصل على اسم الدالة من جانب العميل التي تُستدعى عند تحديث قيمة الخلية. |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | يحصل على الدالة من جانب العميل التي تُستدعى عند إظهار قائمة السياق. |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | يحصل على الدالة من جانب العميل التي تُستدعى عند النقر المزدوج على خلية. |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | يحصل على الدالة من جانب العميل التي تُستدعى عند النقر المزدوج على صف. |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | يحصل على اسم الدالة من جانب العميل التي تُستدعى عند تهيئة الشبكة. |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | يحصل على الدالة من جانب العميل التي تُستدعى بعد تغيير فهرس الصفحة. لا تُطبق إلا عندما يكون EnablePaging صحيحًا. |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | يحصل على الدالة من جانب العميل التي تُستدعى قبل إرسال الصفحة من جانب العميل. |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | يحصل على الدالة الجانبية للعميل التي سيتم استدعاؤها عند تحديد شكل. |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | يحصل على الدالة الجانبية للعميل التي سيتم استدعاؤها قبل إرسال التحكم على جانب العميل. |
| [getOnlyAuto()](#getOnlyAuto--) | يحصل على ما إذا كان يقتصر فقط على ملاءمة الصفوف التي ارتفاعها غير مخصص، القيمة الافتراضية هي false. |
| [getPageSize()](#getPageSize--) | يحصل على حجم الصفحة في وضع التصفح. |
| [getPictureCachePath()](#getPictureCachePath--) | يحصل على مسار تخزين الصور لدفتر العمل، سيتم تخزين جميع الأشكال والصور في هذا الدليل، المسار الافتراضي هو acwcache تحت دليل قاعدة التطبيق الحالي، يحتاج المستخدمون إلى تنفيذ خدمة جدولة لتنظيف الملفات التي انتهت مدة الجلسة. |
| [getPresetStyle()](#getPresetStyle--) | يحصل على النمط المسبق. |
| [getRefreshValidation()](#getRefreshValidation--) | يحصل على ما إذا كان يجب تحديث قيمة التحقق بعد تغيير قيمة الخلية. |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | يحصل على ما إذا كان الصف المخفي يُعرض في GridControl، القيمة الافتراضية هي false. |
| [getRowHeightForCSV()](#getRowHeightForCSV--) | يحصل على قيمة ارتفاع الصف بالنقطة لملف csv، القيمة الافتراضية هي 14.5. |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | يحدد لون زر السهم لشريط التمرير. |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | يحدد لون شريط التمرير للعنصر. |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | يحدد لون خلفية الخلايا المحددة في نطاق التحديد المتعدد. |
| [getSelectCellColor()](#getSelectCellColor--) | يحدد لون الخلايا المحددة في نطاق التحديد المتعدد. |
| [getSessionStorePath()](#getSessionStorePath--) | يحصل على مسار تخزين ذاكرة التخزين المؤقت للجلسة عندما يكون وضع الجلسة File أو ViewState، إلخ: gridweb.SessionStorePath=\"c:/mytempdir/session\"؛ ثم سيخزن بيانات الجلسة في c:/mytempdir/session |
| [getSettings()](#getSettings--) | يمثل إعدادات المصنف. |
| [getShowAddButton()](#getShowAddButton--) | يحصل على ما إذا كان سيتم عرض زر إضافة ورقة العمل. |
| [getShowBottomBar()](#getShowBottomBar--) | يحدد ما إذا كان سيتم عرض شريط الأوامر (يشمل شريط الأوامر وشريط التبويب) في أسفل العنصر. |
| [getShowCellEditBox()](#getShowCellEditBox--) | ما إذا كان Gridweb يعرض شريط أدوات صندوق التحرير كما في MS-EXCEL. إذا تم التفعيل، سيظهر صندوق تحرير للخلية الحالية في Gridweb. |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | يحدد ما إذا كان سيتم عرض شريط الأوامر (يشمل شريط الأوامر وشريط التبويب) في أعلى العنصر. |
| [getShowContextMenu()](#getShowContextMenu--) | يحصل على ما إذا كان سيتم عرض قائمة السياق. القيمة الافتراضية هي true. |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | يحصل على ما إذا كان سيتم عرض خطوط الشبكة الافتراضية للخلايا. |
| [getShowHeaderBar()](#getShowHeaderBar--) | يحصل على ما إذا كان سيتم عرض شريط الرأس |
| [getShowLoading()](#getShowLoading--) | يحدد ما إذا كان سيتم عرض مربع حوار التحميل أثناء الإرسال إلى الخادم. |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | يحدد الموضع الأيسر والعلوي (بالبكسل) لعرض مربع حوار التحميل أثناء الإرسال إلى الخادم، إلخ. 100,200 يعني أن موضع مربع حوار التحميل الأيسر والعلوي هو 100px,200px. |
| [getShowSaveButton()](#getShowSaveButton--) | يحصل على ما إذا كان سيتم عرض زر الحفظ. |
| [getShowSubmitButton()](#getShowSubmitButton--) | يُرجع ما إذا كان زر الإرسال سيظهر. |
| [getShowTabBar()](#getShowTabBar--) | يُرجع ما إذا كان شريط التبويبات سيظهر. |
| [getShowTabNavigation()](#getShowTabNavigation--) | يُرجع ما إذا كان زر تنقل التبويب معروضًا، القيمة الافتراضية هي true. |
| [getShowUndoButton()](#getShowUndoButton--) | يُرجع ما إذا كان زر التراجع سيظهر. |
| [getSpanWrap()](#getSpanWrap--) | يحدد ما إذا كان سيتم لف المحتوى داخل امتداد الخلية، القيمة الافتراضية هي true. |
| [getTabIndex()](#getTabIndex--) | يحصل على TabIndex في WebControl |
| [getTabStyle()](#getTabStyle--) | يُرجع نمط شريط التبويبات. |
| [getToolTip()](#getToolTip--) | يحصل على ToolTip في WebControl |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | يُرجع ما إذا كان GridWeb يستخدم ارتفاع صفحة العميل كارتفاع للتحكم، مناسب عندما يتم تعيين Height="100%", القيمة الافتراضية هي false. |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | يُرجع موضع شريط التمرير في لوحة عرض الشبكة. |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | يُرجع موضع شريط التمرير في لوحة عرض الشبكة. |
| [getViewTableStyle()](#getViewTableStyle--) | يُرجع نمط لوحة عرض البيانات. |
| [getWidth()](#getWidth--) | يُرجع عرض (System.Web.UI.WebControl.Unit) للتحكم. |
| [getWorkSheets()](#getWorkSheets--) | يُرجع مجموعة أوراق العمل. |
| [getXhtmlMode()](#getXhtmlMode--) | يُرجع ما إذا كان سيتم استخدام نمط XHTML، القيمة الافتراضية هي true. |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | يستورد من تدفق ملف إكسل، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة. |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | يستورد من تدفق ملف إكسل، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | يستورد من ملف إكسل. |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | يستورد من ملف إكسل. |
| [isCalculateFormula()](#isCalculateFormula--) | يُرجع ما إذا كان سيتم حساب الصيغة بعد تغيير قيمة الخلية أو بعد استيراد الملف. |
| [loadCSVFile(InputStream stream)](#loadCSVFile-java.io.InputStream-) | يحمّل البيانات من تدفق ملف CSV. |
| [loadCSVFile(String fileName)](#loadCSVFile-java.lang.String-) | يحمّل البيانات من ملف CSV. |
| [loadHTMLFile(InputStream stream)](#loadHTMLFile-java.io.InputStream-) | يحمّل البيانات من تدفق ملف HTML. |
| [loadHTMLFile(String fileName)](#loadHTMLFile-java.lang.String-) | يحمّل البيانات من ملف HTML. |
| [loadSpreadSheetMLFile(InputStream stream)](#loadSpreadSheetMLFile-java.io.InputStream-) | يحمّل البيانات من تدفق ملف SpreadSheetML. |
| [loadSpreadSheetMLFile(String fileName)](#loadSpreadSheetMLFile-java.lang.String-) | يحمّل البيانات من ملف SpreadSheetML. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshChartShape()](#refreshChartShape--) | تحديث جميع صور المخططات للورقة النشطة. |
| [saveCSVFile(OutputStream stream)](#saveCSVFile-java.io.OutputStream-) | يحفظ البيانات إلى تدفق ملف CSV. |
| [saveCSVFile(String targetFile)](#saveCSVFile-java.lang.String-) | يحفظ البيانات إلى ملف CSV. |
| [saveCustomStyleFile(String fileName)](#saveCustomStyleFile-java.lang.String-) | يحفظ بيانات النمط الحالي للتحكم إلى ملف XML. |
| [saveHTMLFile(OutputStream stream)](#saveHTMLFile-java.io.OutputStream-) | يحفظ البيانات إلى تدفق ملف HTML. |
| [saveHTMLFile(String targetFile)](#saveHTMLFile-java.lang.String-) | يحفظ البيانات إلى ملف HTML. |
| [saveSpreadSheetMLFile(OutputStream stream)](#saveSpreadSheetMLFile-java.io.OutputStream-) | يحفظ البيانات إلى تدفق ملف SpreadSheetML. |
| [saveSpreadSheetMLFile(String targetFile)](#saveSpreadSheetMLFile-java.lang.String-) | يحفظ البيانات إلى ملف SpreadSheetML. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | يحفظ أوراق العمل إلى ملف إكسل. |
| [saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)](#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-) | يحفظ أوراق العمل إلى ملف إكسل. |
| [saveToExcelFile(OutputStream stream, int format)](#saveToExcelFile-java.io.OutputStream-int-) | يحفظ أوراق العمل إلى ملف إكسل. |
| [saveToExcelFile(String targetFile)](#saveToExcelFile-java.lang.String-) | يحفظ أوراق العمل إلى ملف إكسل بتنسيق Excel 2003. |
| [saveToExcelFile(String targetFile, GridSaveOptions saveOptions)](#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-) | يحفظ أوراق العمل إلى ملف إكسل. |
| [saveToExcelFile(String targetFile, int format)](#saveToExcelFile-java.lang.String-int-) | يحفظ أوراق العمل إلى ملف إكسل. |
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | يضبط مسار الويب لملفات السكريبت/الصورة الخاصة بالتحكم. |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | يضبط عنوان URL الويب لملف اللغة الخاص بالتحكم. |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | يضبط الخلية النشطة للورقة الحالية. |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | يحدد لون الخلفية للخلية النشطة. |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | يحدد لون الخلية النشطة. |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | يحدد لون الخلفية لرأس الصف/العمود النشط. |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | يحدد لون رأس الصف/العمود النشط. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | يضبط فهرس الورقة النشطة. |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | يحدد نمط التبويب النشط. |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | يضبط ما إذا كان يتم تحديث صورة المخطط أثناء تحديث قيمة الخلية. القيمة الافتراضية هي true. |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | يضبط BackColor في WebControl |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | يضبط BorderColor في WebControl |
| [setBorderStyle(int value)](#setBorderStyle-int-) | يضبط BorderStyle في WebControl |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | يضبط BorderWidth في WebControl |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | يضبط نمط الشريط السفلي للتحكم. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | يضبط ما إذا كان يتم حساب الصيغة بعد تغيّر قيمة الخلية أو بعد استيراد الملف. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | يضبط CssClass في WebControl |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | يضبط فهرس الصفحة الحالية في وضع التصفح. |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | يمثل محرك حساب مخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells. |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | يضبط ملف النمط المخصص من التدفق بما في ذلك تدفق ملف القرص أو تدفق الذاكرة. |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | يضبط اسم ملف النمط المخصص. |
| [setDPI(double value)](#setDPI-double-) | يحصل على / يضبط DPI للجهاز. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | يضبط اسم الخط الافتراضي للعنصر. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | يضبط حجم الخط الافتراضي للتحكم. |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | يضبط لون خط الشبكة الافتراضي. |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | يضبط ما إذا كان يتم عرض النصائح. القيمة الافتراضية هي true. |
| [setEditMode(boolean value)](#setEditMode-boolean-) | يضبط وضع التحرير للتحكم. |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | يضبط ما إذا كان يتم استخدام استدعاء AJAX. القيمة الافتراضية هي true. |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | يضبط ما إذا كان يتم تحميل بيانات الخلايا بطريقة غير متزامنة، يُنصح بتطبيق ذلك على ورقة واحدة تحتوي على أكثر من 10000 خلية. |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | يضبط ما إذا كان يتم تمكين عمليات الأعمدة على جانب العميل. |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | يضبط ما إذا كان يتم تمكين عمليات التجميد على جانب العميل. |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | يضبط ما إذا كان يتم تمكين عمليات الدمج على جانب العميل. |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | يحدد ما إذا كان سيتم تمكين تعديل حجم الأعمدة والصفوف من جانب العميل. |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | يحدد ما إذا كان سيتم تمكين عمليات الصف من جانب العميل. |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | يحدد ما إذا كان سيتم تمكين حدث النقر المزدوج من جانب العميل. |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | يحدد ما إذا كان سيتم تطبيق تأثير الضوء المعدني. |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | يحدد ما إذا كان سيتم تمكين وضع ترقيم الصفحات للعنصر. |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | يحدد ما إذا كان سيتم تمكين مربع حوار النمط من جانب العميل. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | يضبط Enabled في WebControl |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | يحدد ما إذا كان سيتم تمكين الترقيم بعد تصفية البيانات، سيصبح ساريًا عندما تكون EnablePaging صحيحة. |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | يحدد ما إذا كان سيتم فرض التحقق من الصحة من جانب العميل. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | يضبط ForeColor في WebControl |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | يحدد نمط الإطار للعنصر. |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | يحدد ما إذا كان GridWeb سيقوم بعملية الحفظ الافتراضية، القيمة الافتراضية هي true. |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) | يحدد ارتفاع (System.Web.UI.WebControl.Unit) شريط الرأس العلوي للعنصر. |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | يحدد نمط شريط الرأس. |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | يحدد نمط شريط الرأس للعنصر. |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) | يحدد عرض (System.Web.UI.WebControl.Unit) شريط الرأس الأيسر للعنصر. |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | يحدد ارتفاع (System.Web.UI.WebControl.Unit) للعنصر. |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | يحدد ما إذا كان GridWeb سيتجاهل إظهار الصفوف أو الأعمدة التي لا تحتوي على قيم خلايا ولكنها لا تزال مُنسقة. |
| [setLoadOptions(GridLoadOptions value)](#setLoadOptions-com.aspose.gridweb.GridLoadOptions-) | يمثل خيارات التحميل لـ GridWeb. |
| [setMaxColumn(int value)](#setMaxColumn-int-) | يحدد الحد الأقصى لمؤشر العمود المعروض (مبني على الصفر) لورقة الويب. |
| [setMaxRow(int value)](#setMaxRow-int-) | يحدد الحد الأقصى لمؤشر الصف المعروض (مبني على الصفر) لورقة الويب. |
| [setMessage(String value)](#setMessage-java.lang.String-) | يحدد الرسالة للشبكة. |
| [setMinColumn(int value)](#setMinColumn-int-) | يحدد الحد الأدنى لمؤشر العمود المعروض (مبني على الصفر) لورقة الويب. |
| [setMinRow(int value)](#setMinRow-int-) | يحدد الحد الأدنى لمؤشر الصف المعروض (مبني على الصفر) لورقة الويب. |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | يحدد ما إذا كان سيتم إظهار صفوف المجموعات. |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | يحدد قيمة تشير إلى ما إذا كان شريط التمرير الأفقي مخفيًا. |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | يحدد ما إذا كان سيتم إظهار شريط التمرير. |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | يحدد قيمة تشير إلى ما إذا كان شريط التمرير العمودي مخفيًا. |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | يضبط اسم الدالة على جانب العميل التي تُستدعى عند انتهاء استدعاء ajax. |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | يضبط اسم الدالة على جانب العميل التي تُستدعى عندما تفشل صلاحية الخلية. |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | يضبط الدالة على جانب العميل التي تُستدعى عند تحديد خلية. |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | يضبط الدالة على جانب العميل التي تُستدعى عند تحديد خلية. |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | يضبط الدالة على جانب العميل التي تُستدعى عند إلغاء تحديد خلية. |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | يضبط اسم الدالة على جانب العميل التي تُستدعى عند تحديث قيمة الخلية. |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | يضبط الدالة على جانب العميل التي تُستدعى عند إظهار قائمة السياق. |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | يضبط الدالة على جانب العميل التي تُستدعى عند النقر المزدوج على خلية. |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | يضبط الدالة على جانب العميل التي تُستدعى عند النقر المزدوج على صف. |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | يضبط اسم الدالة على جانب العميل التي تُستدعى عند تهيئة الشبكة. |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | يضبط الدالة على جانب العميل التي تُستدعى بعد تغيير فهرس الصفحة. لا تُطبق إلا عندما تكون EnablePaging مفعلة. |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | يضبط الدالة على جانب العميل التي تُستدعى قبل إرسال الصفحة من جانب العميل. |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | يضبط الدالة على جانب العميل التي تُستدعى عند تحديد شكل. |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | يضبط الدالة على جانب العميل التي تُستدعى قبل إرسال التحكم من جانب العميل. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | يضبط ما إذا كان يتم ضبط الصفوف التي ارتفاعها غير مخصص فقط، القيمة الافتراضية هي false. |
| [setPageSize(int value)](#setPageSize-int-) | يضبط حجم الصفحة في وضع التقسيم. |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | يضبط مسار تخزين الصور لدفتر العمل، جميع الأشكال والصور ستُخزن في هذا الدليل، المسار الافتراضي هو acwcache داخل دليل قاعدة التطبيق الحالي، يحتاج المستخدمون إلى تنفيذ خدمة جدولة لتنظيف الملفات التي انتهى وقت جلسةها. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | يضبط النمط المسبق. |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | يضبط ما إذا كان سيتم تحديث قيمة التحقق بعد تغيير قيمة الخلية. |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | يضبط ما إذا كان الصف المخفي يُعرض في GridControl، القيمة الافتراضية هي false. |
| [setRowHeightForCSV(double value)](#setRowHeightForCSV-double-) | يضبط قيمة ارتفاع الصف بالنقطة لملف csv، القيمة الافتراضية هي 14.5. |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | يحدد لون زر السهم لشريط التمرير. |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | يحدد لون شريط التمرير للعنصر. |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | يحدد لون خلفية الخلايا المحددة في نطاق التحديد المتعدد. |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | يحدد لون الخلايا المحددة في نطاق التحديد المتعدد. |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | يضبط مسار تخزين ذاكرة التخزين المؤقت للجلسة عندما يكون وضع الجلسة File أو ViewState، إلخ: gridweb.SessionStorePath="c:/mytempdir/session"؛ ثم سيُخزن بيانات الجلسة في c:/mytempdir/session. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | يمثل إعدادات المصنف. |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | يضبط ما إذا كان سيتم إظهار زر إضافة ورقة العمل. |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | يحدد ما إذا كان سيتم عرض شريط الأوامر (يشمل شريط الأوامر وشريط التبويب) في أسفل العنصر. |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | ما إذا كان Gridweb يعرض شريط أدوات صندوق التحرير كما في MS-EXCEL. إذا تم التفعيل، سيظهر صندوق تحرير للخلية الحالية في Gridweb. |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | يحدد ما إذا كان سيتم عرض شريط الأوامر (يشمل شريط الأوامر وشريط التبويب) في أعلى العنصر. |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | يضبط ما إذا كان سيتم إظهار قائمة السياق. القيمة الافتراضية هي true. |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | يضبط ما إذا كان سيتم إظهار خطوط الشبكة الافتراضية للخلية. |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | يضبط ما إذا كان سيتم إظهار شريط العنوان |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | يحدد ما إذا كان سيتم عرض مربع حوار التحميل أثناء الإرسال إلى الخادم. |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | يحدد الموضع الأيسر والعلوي (بالبكسل) لعرض مربع حوار التحميل أثناء الإرسال إلى الخادم، إلخ. 100,200 يعني أن موضع مربع حوار التحميل الأيسر والعلوي هو 100px,200px. |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | يضبط ما إذا كان سيتم عرض زر الحفظ. |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | يضبط ما إذا كان سيتم عرض زر الإرسال. |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | يضبط ما إذا كان سيتم عرض شريط علامات التبويب. |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | يضبط ما إذا كان زر تنقل علامات التبويب معروضًا، القيمة الافتراضية هي true. |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | يضبط ما إذا كان سيتم عرض زر التراجع. |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | يحدد ما إذا كان سيتم لف المحتوى داخل امتداد الخلية، القيمة الافتراضية هي true. |
| [setTabIndex(short value)](#setTabIndex-short-) | يضبط TabIndex في WebControl |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | يضبط نمط شريط علامات التبويب. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | يضبط ToolTip في WebControl |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | يضبط ما إذا كان GridWeb يستخدم ارتفاع صفحة العميل كارتفاع للعنصر، مناسب عندما يتم تعيين Height=\"100%\", القيمة الافتراضية هي false. |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | يضبط موضع شريط التمرير في لوحة عرض الشبكة. |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | يضبط موضع شريط التمرير في لوحة عرض الشبكة. |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | يضبط نمط لوحة عرض البيانات. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | يضبط عرض (System.Web.UI.WebControl.Unit) للعنصر. |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | يضبط ما إذا كان سيتم استخدام نمط XHTML، القيمة الافتراضية هي true. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MainWeb() {#MainWeb--}
```
public MainWeb()
```


البناء الافتراضي لـ control MainWeb.

### AfterColumnFilter {#AfterColumnFilter}
```
public RowColumnEventHandler AfterColumnFilter
```


يحدث بعد تصفية العمود.

### AjaxCallFinished {#AjaxCallFinished}
```
public WorkbookEventHandler AjaxCallFinished
```


يتم إطلاقه عندما ينتهي تحديث الـ ajax للعنصر. (يجب تعيين EnableAJAX إلى true)

### BeforeColumnFilter {#BeforeColumnFilter}
```
public RowColumnEventHandler BeforeColumnFilter
```


يحدث قبل تصفية العمود.

### CellClickOnAjax {#CellClickOnAjax}
```
public CellEventStringHandler CellClickOnAjax
```


يحدث عندما يتم النقر على الخلية، ويحتاج إلى إجراء ajaxcallback لهذا الحدث.

### CellClientUpdate {#CellClientUpdate}
```
public CellEventHandler CellClientUpdate
```


يحدث عندما يحدث تحديث خلية للعميل. عندما يتم إطلاق هذا الحدث، يحتوي المتغير e.Argument على اسم الأمر.

### CellCommand {#CellCommand}
```
public CellEventHandler CellCommand
```


يحدث عندما يتم النقر على ارتباط الأمر للخلية. عندما يتم إطلاق هذا الحدث، يحتوي المتغير e.Argument على اسم الأمر.

### CellDoubleClick {#CellDoubleClick}
```
public CellEventHandler CellDoubleClick
```


يحدث عندما يتم النقر المزدوج على الخلية.

### CellModifiedOnAjax {#CellModifiedOnAjax}
```
public CellEventHandler CellModifiedOnAjax
```


يحدث عندما يتم تعديل الخلية في ajaxcall.

### ColumnDeleted {#ColumnDeleted}
```
public RowColumnEventHandler ColumnDeleted
```


يحدث عندما يحذف المستخدم عمودًا من القائمة الجانبية للعميل.

### ColumnDeleting {#ColumnDeleting}
```
public RowColumnEventHandler ColumnDeleting
```


يحدث عندما يحاول المستخدم حذف عمود من القائمة الجانبية للعميل. يمكنك معالجة هذا الحدث وتعيين المتغير cancel إلى True لإلغاء عملية الحذف.

### ColumnDoubleClick {#ColumnDoubleClick}
```
public RowColumnEventHandler ColumnDoubleClick
```


يحدث عندما يتم النقر المزدوج على رأس العمود.

### ColumnInserted {#ColumnInserted}
```
public RowColumnEventHandler ColumnInserted
```


يحدث عندما يُدخل المستخدم عمودًا من القائمة الجانبية للعميل.

### CustomCommand {#CustomCommand}
```
public CustomCommandEventHandler CustomCommand
```


يحدث عندما ينقر المستخدم على زر أمر مخصص.

### LoadCustomData {#LoadCustomData}
```
public WorkbookEventHandler LoadCustomData
```


يتم إطلاقه عندما يتم تعيين SessionMode للعنصر إلى Custom ويحتاج إلى تحميل بيانات الورقة. يمكنك معالجة هذا الحدث في وضع الجلسة المخصص لتحميل بيانات الورقة من ملف أو قاعدة بيانات.

### PageIndexChanged {#PageIndexChanged}
```
public WorkbookEventHandler PageIndexChanged
```


يحدث عندما يتغير فهرس صفحة الورقة في التحكم.

### RowDeleted {#RowDeleted}
```
public RowColumnEventHandler RowDeleted
```


يحدث عندما يقوم المستخدم بحذف صف من القائمة الجانبية للعميل.

### RowDeleting {#RowDeleting}
```
public RowColumnEventHandler RowDeleting
```


يحدث عندما يحاول المستخدم حذف صف من القائمة الجانبية للعميل. يمكنك معالجة هذا الحدث ورمي استثناء RejectDeleteException لإلغاء عملية الحذف.

### RowDoubleClick {#RowDoubleClick}
```
public RowColumnEventHandler RowDoubleClick
```


يحدث عندما يتم النقر المزدوج على رأس الصف.

### RowInserted {#RowInserted}
```
public RowColumnEventHandler RowInserted
```


يحدث عندما يقوم المستخدم بإدراج صف من القائمة الجانبية للعميل.

### SaveCommand {#SaveCommand}
```
public WorkbookEventHandler SaveCommand
```


يحدث عندما يتم النقر على زر "save".

### SheetAdded {#SheetAdded}
```
public SheetEventHandler SheetAdded
```


يحدث عندما يضيف المستخدم ورقة عمل من قائمة شريط الأدوات.

### SheetTabClick {#SheetTabClick}
```
public WorkbookEventHandler SheetTabClick
```


يحدث عندما يتم النقر على تبويب الورقة.

### SubmitCommand {#SubmitCommand}
```
public WorkbookEventHandler SubmitCommand
```


يحدث عندما يتم النقر على زر "submit".

### UndoCommand {#UndoCommand}
```
public WorkbookEventHandler UndoCommand
```


يحدث عندما يتم النقر على زر "undo".

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


يحسب نتيجة الصيغ.

### createChildControls() {#createChildControls--}
```
public void createChildControls()
```


تنفيذ CreateChildControls من WebControl، يستخدم داخليًا فقط.

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
### getACWClientPath() {#getACWClientPath--}
```
public String getACWClientPath()
```


يحصل على مسار الويب لملفات السكريبت/الصورة للعنصر. على سبيل المثال: \"http://localhost/acw\\_client\". يمكنك أيضًا تعيين هذه القيمة في ملف web.config. أضف هذا القسم إلى قسم `<configuration>`:
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```


يحصل على عنوان URL للغة للملف الخاص بالعنصر. على سبيل المثال: \"/acw\\_client/lang\\_en.js\".
بشكل افتراضي، يتم استخدام ملف إنجليزي مدمج.


**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```


يحصل على الخلية النشطة في الورقة الحالية. تم تعديلها لتكون قابلة للكتابة منذ الإصدار 1.9.0.1.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```


يحدد لون الخلفية للخلية النشطة.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```


يحدد لون الخلية النشطة.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```


يحدد لون الخلفية لرأس الصف/العمود النشط.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```


يحدد لون رأس الصف/العمود النشط.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveSheet() {#getActiveSheet--}
```
public GridWorksheet getActiveSheet()
```


يحصل على الورقة النشطة

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


يحصل على فهرس الورقة النشطة. يساوي WebWorksheets.ActiveSheetIndex.

**Returns:**
int
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```


يحدد نمط التبويب النشط.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getAutoRefreshChart() {#getAutoRefreshChart--}
```
public boolean getAutoRefreshChart()
```


يحصل على ما إذا كانت صورة Chart يتم تحديثها أثناء تحديث قيمة الخلية. القيمة الافتراضية هي true

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


يحصل على BackColor في WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


يحصل على BorderColor في WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


يحصل على BorderStyle في WebControl

انظر [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


يحصل على BorderWidth في WebControl

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```


يحصل على نمط الشريط السفلي للتحكم.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


يحصل على CssClass في WebControl

**Returns:**
java.lang.String
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```


يحصل على فهرس الصفحة الحالية في وضع التصفح.

**Remarks**

عند تشغيل وضع الصفحات، سيعرض التحكم PageSize صفوف من البيانات مرة واحدة، ويعرض عنصر التحكم لتحديد الصفحة في شريط التبويب.

**Returns:**
int
### getCustomCalculationEngine() {#getCustomCalculationEngine--}
```
public GridAbstractCalculationEngine getCustomCalculationEngine()
```


يمثل محرك حساب مخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

**Returns:**
[GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine)
### getCustomCommandButtons() {#getCustomCommandButtons--}
```
public CustomCommandButtonCollection getCustomCommandButtons()
```


يحصل على مجموعة أزرار الأوامر المخصصة

**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```


يحصل على اسم ملف النمط المخصص.

**Remarks**

ملف النمط المخصص هو ملف XML. عند تعيين اسم الملف، سيتم تحميل الملف فورًا. هنا محتوى "النمط المسبق القياسي" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Example**

```
         		GridWeb1.setCustomStyleFileName("c:\\style\\mystyle.xml");
```

**Returns:**
java.lang.String
### getDPI() {#getDPI--}
```
public static double getDPI()
```


يحصل على / يضبط DPI للجهاز.

**Remarks**

**Returns:**
double
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


يحصل على اسم الخط الافتراضي للعنصر.

**Example**

```
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


يحصل على حجم الخط الافتراضي للعنصر.

**Example**

```
         		GridWeb1.setDefaultFontSize(new FontUnit("10pt"));
```

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getDefaultGridLineColor() {#getDefaultGridLineColor--}
```
public Color getDefaultGridLineColor()
```


يحصل على لون خط الشبكة الافتراضي.

**Example**

```
         		GridWeb1.setDefaultGridLineColor(Color.getRed());
```

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getDisplayCellTip() {#getDisplayCellTip--}
```
public boolean getDisplayCellTip()
```


يحصل على ما إذا كان سيتم إظهار التلميحات. القيمة الافتراضية هي true.

**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```


يحصل على وضع التحرير للعنصر.

**Remarks**

عند تعيينه إلى true، خلايا التحكم قابلة للتحرير، ويتم عرض أيقونتي "save" و "undo". عند تعيينه إلى false، تكون خلايا التحكم للقراءة فقط، ولا يتم عرض أيقونتي "save" و "undo".

**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```


يحصل على ما إذا كان سيتم استخدام استدعاء AJAX. القيمة الافتراضية هي true.

**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```


يحصل على ما إذا كان سيتم تحميل بيانات الخلايا بطريقة غير متزامنة، يُنصح بتطبيق ذلك على ورقة واحدة تحتوي على أكثر من 10000 خلية.

**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```


يحصل على ما إذا كان سيتم تمكين عمليات الأعمدة على جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم استخدام قائمة النقر بزر الفأرة الأيمن لإضافة/إزالة الأعمدة.

**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```


يحصل على ما إذا كان سيتم تمكين عمليات التجميد على جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم استخدام قائمة النقر بزر الفأرة الأيمن لتجميد/إلغاء تجميد الألواح.

**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```


يحصل على ما إذا كان سيتم تمكين عمليات الدمج على جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم استخدام قائمة النقر بزر الفأرة الأيمن لدمج/فصل الخلايا.

**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```


يحصل على ما إذا كان سيتم تمكين تغيير حجم الأعمدة والصفوف على جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم تغيير حجم العمود والصف على جانب العميل.

**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```


يحصل على ما إذا كان سيتم تمكين عمليات الصفوف على جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم استخدام قائمة النقر بزر الفأرة الأيمن لإضافة/إزالة الصفوف.

**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```


يحصل على ما إذا كان سيتم تمكين حدث النقر المزدوج على جانب العميل.

**Remarks**

عند تعيينه إلى true، سيتلقى التحكم أحداث النقر المزدوج على جانب العميل ويمكنك معالجة هذه الأحداث على جانب الخادم. وإلا سيتجاهل التحكم أي أحداث نقر مزدوج.

**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```


يحصل على ما إذا كان سيتم تطبيق تأثير الضوء المعدني.

**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```


يحصل على ما إذا كان سيتم تمكين وضع الصفحات للعنصر.

**Remarks**

عند تعيينه إلى true، سيعرض التحكم عدد صفوف PageSize من البيانات مرة واحدة، ويعرض عنصر التحكم لاختيار الصفحة في شريط التبويب.

**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```


يحصل على ما إذا كان سيتم تمكين مربع حوار النمط على جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم استخدام مربع حوار النمط لتعيين نمط الخلية عن طريق اختيار "Format Cell..." من القائمة المنبثقة.

**Returns:**
boolean
### getEnabled() {#getEnabled--}
```
public boolean getEnabled()
```


يحصل على Enabled في WebControl

**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```


يحصل على ما إذا كان سيتم تمكين الصفحات بعد تصفية البيانات، سيصبح ساريًا عندما تكون EnablePaging true.

**Remarks**

عند تعيينه إلى true، سيقوم التحكم بالترقيم بناءً على البيانات المفلترة، القيمة الافتراضية هي false.

**Returns:**
boolean
### getFont() {#getFont--}
```
public FontInfo getFont()
```


يحصل على Font في WebControl

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```


يحصل على ما إذا كان سيتم فرض التحقق على جانب العميل.

**Remarks**

عند تعيينه إلى true، لن يتم إرسال البيانات إلى الخادم حتى تكون جميع حقول الإدخال صالحة.

**Returns:**
boolean
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


يحصل على ForeColor في WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```


يحصل على نمط الإطار للعنصر.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```


يحصل على ما إذا كان GridWeb سيقوم بعملية الحفظ الافتراضية، القيمة الافتراضية هي true.

**Returns:**
boolean
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```


يحصل على ارتفاع (System.Web.UI.WebControl.Unit) شريط الرأس العلوي للعنصر.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeaderBarStyle() {#getHeaderBarStyle--}
```
public GridTableItemStyle getHeaderBarStyle()
```


يحصل على نمط شريط الرأس.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```


يحصل على نمط شريط الرأس للعنصر

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```


يحصل على عرض ( System.Web.UI.WebControl.Unit ) أو شريط الرأس الأيسر للعنصر.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


يحصل على ارتفاع ( System.Web.UI.WebControl.Unit ) للعنصر.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getIgnoreStyleWithNoData() {#getIgnoreStyleWithNoData--}
```
public boolean getIgnoreStyleWithNoData()
```


يحدد ما إذا كان GridWeb يتجاهل إظهار الصفوف أو الأعمدة التي لا تحتوي على قيم خلايا ولكنها ما زالت مُنسقة. إذا تم تعيينه إلى true، ستكون الأداء أفضل. القيمة الافتراضية هي false، مما يعني أنه إذا كان الصف/العمود المتتالي الأخير لا يحتوي على قيم خلايا ولكنه مُنسق، فسنظل نعرضه. هذا الخيار صالح فقط عندما يكون EnableAsync مساويًا لـ false. لا يؤثر هذا الخيار عندما يكون EnableAsync مساويًا لـ true، مما يعني أن GridWeb سيعرض جميع الصفوف/الأعمدة مع النمط.

**Returns:**
boolean
### getLoadOptions() {#getLoadOptions--}
```
public GridLoadOptions getLoadOptions()
```


يمثل خيارات التحميل لـ GridWeb.

**Returns:**
[GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


يحدد الحد الأقصى لمؤشر العمود المعروض (مؤشر صفر) في ورقة الويب. يستخدم التحكم القيمة الأكبر بين MaxColumn والحد الأقصى للعمود في بيانات الورقة.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


يحدد الحد الأقصى لمؤشر الصف المعروض (مؤشر صفر) في ورقة الويب. يستخدم التحكم القيمة الأكبر بين MaxRow والحد الأقصى للصف في بيانات الورقة.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMessage() {#getMessage--}
```
public String getMessage()
```


يحصل على الرسالة الخاصة بالشبكة.

**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


يحدد الحد الأدنى لمؤشر العمود المعروض (مؤشر صفر) في ورقة الويب. يستخدم التحكم القيمة الأصغر بين MinColumn والحد الأدنى للعمود في بيانات الورقة.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


يحدد الحد الأدنى لمؤشر الصف المعروض (مؤشر صفر) في ورقة الويب. يستخدم التحكم القيمة الأصغر بين MinRow والحد الأدنى للصف في بيانات الورقة.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getModifiedCells() {#getModifiedCells--}
```
public ArrayList getModifiedCells()
```


يحصل على مجموعة الخلايا التي تم تعديلها من قبل العميل.

**Returns:**
java.util.ArrayList
### getNeedRenderGroupRows() {#getNeedRenderGroupRows--}
```
public boolean getNeedRenderGroupRows()
```


يحصل على ما إذا كان يجب إظهار صفوف المجموعات.

**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```


يحصل على قيمة تشير إلى ما إذا كان شريط التمرير الأفقي مخفيًا.

**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```


يحصل على ما إذا كان يجب إظهار شريط التمرير.

**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```


يحصل على قيمة تشير إلى ما إذا كان شريط التمرير العمودي مخفيًا.

**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```


يحدد اسم الدالة على جانب العميل التي سيتم استدعاؤها عند انتهاء ajaxcall. يجب إعلان الدالة على الجانب العميل كما يلي:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnCellErrorClientFunction() {#getOnCellErrorClientFunction--}
```
public String getOnCellErrorClientFunction()
```


يحدد اسم الدالة على جانب العميل التي سيتم استدعاؤها عندما يفشل التحقق من صحة الخلية. يجب إعلان الدالة على الجانب العميل كما يلي:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```


يحصل على الدالة الجانبية للعميل التي سيتم استدعاؤها عندما يتم تحديد خلية. يجب إعلان الدالة الجانبية للعميل كما يلي:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnCellSelectedClientFunction() {#getOnCellSelectedClientFunction--}
```
public String getOnCellSelectedClientFunction()
```


يحصل على الدالة الجانبية للعميل التي سيتم استدعاؤها عندما يتم تحديد خلية. يجب إعلان الدالة الجانبية للعميل كما يلي:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnCellUnselectedClientFunction() {#getOnCellUnselectedClientFunction--}
```
public String getOnCellUnselectedClientFunction()
```


يحصل على الدالة الجانبية للعميل التي سيتم استدعاؤها عندما يتم إلغاء تحديد خلية. يجب إعلان الدالة الجانبية للعميل كما يلي:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```


يحصل على اسم الدالة الجانبية للعميل التي سيتم استدعاؤها عندما يتم تحديث قيمة الخلية. يجب إعلان الدالة الجانبية للعميل كما يلي:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnContextMenuShowClientFunction() {#getOnContextMenuShowClientFunction--}
```
public String getOnContextMenuShowClientFunction()
```


يحصل على الدالة الجانبية للعميل التي سيتم استدعاؤها عندما يتم عرض قائمة السياق. يجب إعلان الدالة الجانبية للعميل كما يلي:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnDoubleClickCellClientFunction() {#getOnDoubleClickCellClientFunction--}
```
public String getOnDoubleClickCellClientFunction()
```


يحصل على الدالة الجانبية للعميل التي سيتم استدعاؤها عندما يتم النقر المزدوج على خلية. يجب إعلان الدالة الجانبية للعميل كما يلي:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```


يحصل على الدالة الجانبية للعميل التي سيتم استدعاؤها عندما يتم النقر المزدوج على صف. يجب إعلان الدالة الجانبية للعميل كما يلي:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnGridInitClientFunction() {#getOnGridInitClientFunction--}
```
public String getOnGridInitClientFunction()
```


يحصل على اسم الدالة الجانبية للعميل التي سيتم استدعاؤها عندما يتم تهيئة الشبكة. يجب إعلان الدالة الجانبية للعميل كما يلي:
function MyOnGridInit(grid)
\{
alert("The grid is initialized: " + grid.id);
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnPageChangeClientFunction() {#getOnPageChangeClientFunction--}
```
public String getOnPageChangeClientFunction()
```


يحصل على الدالة الجانبية للعميل التي سيتم استدعاؤها بعد تغيير فهرس الصفحة. لا تأخذ تأثيرًا إلا عندما يكون EnablePaging صحيحًا. يجب إعلان الدالة الجانبية للعميل كما يلي:
function MyOnPageChange(index)
\{
console.log("current page is:"+index);
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnPageSubmitClientFunction() {#getOnPageSubmitClientFunction--}
```
public String getOnPageSubmitClientFunction()
```


يحصل على الدالة من جانب العميل التي تُستدعى قبل إرسال الصفحة من جانب العميل.

**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```


يحصل على الدالة الجانبية للعميل التي سيتم استدعاؤها عند اختيار شكل. يجب إعلان دالة العميل كما يلي:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnSubmitClientFunction() {#getOnSubmitClientFunction--}
```
public String getOnSubmitClientFunction()
```


يحصل على دالة العميل التي سيتم استدعاؤها قبل إرسال التحكم من جانب العميل. يجب إعلان دالة العميل كما يلي:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
المتغير arg هو معامل الإرسال، يحتوي على الأمر الذي سيُرسل إلى الخادم. المتغير cancelEdit هو قيمة منطقية تشير إلى ما إذا كان التحكم قد تخلص من إدخال المستخدم قبل الإرسال. سيستمر التحكم في الإرسال إذا أعادت الدالة القيمة true.
ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Returns:**
java.lang.String
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


يحصل على ما إذا كان يقتصر فقط على ملاءمة الصفوف التي ارتفاعها غير مخصص، القيمة الافتراضية هي false.

**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```


يحصل على حجم الصفحة في وضع التصفح.

**Remarks**

عند تشغيل وضع الصفحات، سيعرض التحكم PageSize صفوف من البيانات مرة واحدة، ويعرض عنصر التحكم لتحديد الصفحة في شريط التبويب.

**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```


يحصل على مسار تخزين الصور لدفتر العمل، سيتم تخزين جميع الأشكال والصور في هذا الدليل، المسار الافتراضي هو acwcache تحت دليل قاعدة التطبيق الحالي، يحتاج المستخدمون إلى تنفيذ خدمة جدولة لتنظيف الملفات التي انتهت مدة الجلسة.

**Returns:**
java.lang.String
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


يحصل على النمط المسبق.

انظر [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Example**

```
         		GridWeb1.setPresetStyle(PresetStyle.TRADITIONAL_1);
```

**Returns:**
int
### getRefreshValidation() {#getRefreshValidation--}
```
public boolean getRefreshValidation()
```


يحصل على ما إذا كان يجب تحديث قيمة التحقق بعد تغيير قيمة الخلية.

**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```


يحدد ما إذا كان الصف المخفي يُعرض في GridControl، القيمة الافتراضية هي false. إذا كنت بحاجة إلى إظهار الصف المخفي لاحقًا، يجب تعيينه إلى true.

**Returns:**
boolean
### getRowHeightForCSV() {#getRowHeightForCSV--}
```
public double getRowHeightForCSV()
```


يحصل على قيمة ارتفاع الصف بالنقطة لملف csv، القيمة الافتراضية هي 14.5.

**Returns:**
double
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```


يحدد لون زر السهم لشريط التمرير.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```


يحدد لون شريط التمرير للعنصر.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```


يحدد لون خلفية الخلايا المحددة في نطاق التحديد المتعدد.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```


يحدد لون الخلايا المحددة في نطاق التحديد المتعدد.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```


يحصل على مسار تخزين ذاكرة التخزين المؤقت للجلسة عندما يكون وضع الجلسة File أو ViewState، إلخ: gridweb.SessionStorePath=\"c:/mytempdir/session\"؛ ثم سيخزن بيانات الجلسة في c:/mytempdir/session

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


يمثل إعدادات المصنف.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```


يحصل على ما إذا كان سيتم عرض زر إضافة ورقة العمل.

**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```


يحدد ما إذا كان سيتم عرض شريط الأوامر (يشمل شريط الأوامر وشريط التبويب) في أسفل العنصر.

**Returns:**
boolean
### getShowCellEditBox() {#getShowCellEditBox--}
```
public boolean getShowCellEditBox()
```


ما إذا كان Gridweb يعرض شريط أدوات مربع التحرير كما في MS-EXCEL. إذا تم التفعيل، سيظهر مربع تحرير للخلية الحالية في Gridweb. عند تفعيل هذه الميزة، نحتاج إلى استيراد مكتبة jquery js في ملفات aspx الخاصة بك لدعم هذه الميزة الجديدة. أي نسخة حديثة من jquery تعمل.

**Returns:**
boolean
### getShowCommandBarAtTop() {#getShowCommandBarAtTop--}
```
public boolean getShowCommandBarAtTop()
```


يحدد ما إذا كان سيتم عرض شريط الأوامر (يشمل شريط الأوامر وشريط التبويب) في أعلى العنصر.

**Returns:**
boolean
### getShowContextMenu() {#getShowContextMenu--}
```
public boolean getShowContextMenu()
```


يحصل على ما إذا كان سيتم عرض قائمة السياق. القيمة الافتراضية هي true.

**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```


يحصل على ما إذا كان سيتم عرض خطوط الشبكة الافتراضية للخلايا.

**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```


يحصل على ما إذا كان سيتم عرض شريط الرأس

**Returns:**
boolean
### getShowLoading() {#getShowLoading--}
```
public boolean getShowLoading()
```


يحدد ما إذا كان سيتم عرض مربع حوار التحميل أثناء الإرسال إلى الخادم.

**Returns:**
boolean
### getShowLoadingPosition() {#getShowLoadingPosition--}
```
public String getShowLoadingPosition()
```


يحدد الموضع الأيسر والعلوي (بالبكسل) لعرض مربع حوار التحميل أثناء الإرسال إلى الخادم، إلخ. 100,200 يعني أن موضع مربع حوار التحميل الأيسر والعلوي هو 100px,200px.

**Returns:**
java.lang.String
### getShowSaveButton() {#getShowSaveButton--}
```
public boolean getShowSaveButton()
```


يحصل على ما إذا كان سيتم عرض زر الحفظ.

**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```


يُرجع ما إذا كان زر الإرسال سيظهر.

**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```


يُرجع ما إذا كان شريط التبويبات سيظهر.

**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```


يُرجع ما إذا كان زر تنقل التبويب معروضًا، القيمة الافتراضية هي true.

**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```


يُرجع ما إذا كان زر التراجع سيظهر.

**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```


يحدد ما إذا كان سيتم لف المحتوى داخل امتداد الخلية، القيمة الافتراضية هي true.

**Returns:**
boolean
### getTabIndex() {#getTabIndex--}
```
public short getTabIndex()
```


يحصل على TabIndex في WebControl

**Returns:**
short
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```


يُرجع نمط شريط التبويبات.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


يحصل على ToolTip في WebControl

**Returns:**
java.lang.String
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```


يُرجع ما إذا كان GridWeb يستخدم ارتفاع صفحة العميل كارتفاع للتحكم، مناسب عندما يتم تعيين Height="100%", القيمة الافتراضية هي false.

**Returns:**
boolean
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```


يُرجع موضع شريط التمرير في لوحة عرض الشبكة.

**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```


يُرجع موضع شريط التمرير في لوحة عرض الشبكة.

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```


يُرجع نمط لوحة عرض البيانات.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


يُرجع عرض (System.Web.UI.WebControl.Unit) للتحكم.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWorkSheets() {#getWorkSheets--}
```
public GridWorksheetCollection getWorkSheets()
```


يُرجع مجموعة أوراق العمل.

**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```


يُرجع ما إذا كان سيتم استخدام نمط XHTML، القيمة الافتراضية هي true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream stream) {#importExcelFile-java.io.InputStream-}
```
public void importExcelFile(InputStream stream)
```


يستورد من تدفق ملف إكسل، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق ملف Excel، بما في ذلك دفق ملف على القرص أو دفق الذاكرة. |

### importExcelFile(InputStream stream, String passwordtoOpen) {#importExcelFile-java.io.InputStream-java.lang.String-}
```
public void importExcelFile(InputStream stream, String passwordtoOpen)
```


يستورد من تدفق ملف إكسل، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق ملف Excel، بما في ذلك دفق ملف على القرص أو دفق الذاكرة. |
| passwordtoOpen | java.lang.String | كلمة المرور لفتح الملف المشفر. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


يستورد من ملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف Excel. |

### importExcelFile(String fileName, String passwordtoOpen) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String fileName, String passwordtoOpen)
```


يستورد من ملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف Excel. |
| passwordtoOpen | java.lang.String | كلمة المرور لفتح الملف المشفر. |

### isCalculateFormula() {#isCalculateFormula--}
```
public boolean isCalculateFormula()
```


يحدد ما إذا كان يتم حساب الصيغة بعد تغيير قيمة الخلية أو بعد استيراد الملف. القيمة الافتراضية هي true.

**Returns:**
boolean
### loadCSVFile(InputStream stream) {#loadCSVFile-java.io.InputStream-}
```
public void loadCSVFile(InputStream stream)
```


يحمّل البيانات من تدفق ملف CSV.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق الملف. |

### loadCSVFile(String fileName) {#loadCSVFile-java.lang.String-}
```
public void loadCSVFile(String fileName)
```


يحمّل البيانات من ملف CSV.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف. |

### loadHTMLFile(InputStream stream) {#loadHTMLFile-java.io.InputStream-}
```
public void loadHTMLFile(InputStream stream)
```


يحمّل البيانات من تدفق ملف HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق الملف. |

### loadHTMLFile(String fileName) {#loadHTMLFile-java.lang.String-}
```
public void loadHTMLFile(String fileName)
```


يحمّل البيانات من ملف HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف. |

### loadSpreadSheetMLFile(InputStream stream) {#loadSpreadSheetMLFile-java.io.InputStream-}
```
public void loadSpreadSheetMLFile(InputStream stream)
```


يحمّل البيانات من تدفق ملف SpreadSheetML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق الملف. |

### loadSpreadSheetMLFile(String fileName) {#loadSpreadSheetMLFile-java.lang.String-}
```
public void loadSpreadSheetMLFile(String fileName)
```


يحمّل البيانات من ملف SpreadSheetML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshChartShape() {#refreshChartShape--}
```
public void refreshChartShape()
```


تحديث جميع صور المخططات للورقة النشطة.

### saveCSVFile(OutputStream stream) {#saveCSVFile-java.io.OutputStream-}
```
public void saveCSVFile(OutputStream stream)
```


يحفظ البيانات إلى تدفق ملف CSV.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الملف. |

### saveCSVFile(String targetFile) {#saveCSVFile-java.lang.String-}
```
public void saveCSVFile(String targetFile)
```


يحفظ البيانات إلى ملف CSV.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| targetFile | java.lang.String | اسم الملف. |

### saveCustomStyleFile(String fileName) {#saveCustomStyleFile-java.lang.String-}
```
public void saveCustomStyleFile(String fileName)
```


يحفظ بيانات النمط الحالية للتحكم في ملف XML. يمكن استخدامه لإنشاء ملف نمط مخصص خاص بك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف النمط. |

### saveHTMLFile(OutputStream stream) {#saveHTMLFile-java.io.OutputStream-}
```
public void saveHTMLFile(OutputStream stream)
```


يحفظ البيانات إلى تدفق ملف HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الملف. |

### saveHTMLFile(String targetFile) {#saveHTMLFile-java.lang.String-}
```
public void saveHTMLFile(String targetFile)
```


يحفظ البيانات إلى ملف HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| targetFile | java.lang.String | اسم الملف. |

### saveSpreadSheetMLFile(OutputStream stream) {#saveSpreadSheetMLFile-java.io.OutputStream-}
```
public void saveSpreadSheetMLFile(OutputStream stream)
```


يحفظ البيانات إلى تدفق ملف SpreadSheetML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الملف. |

### saveSpreadSheetMLFile(String targetFile) {#saveSpreadSheetMLFile-java.lang.String-}
```
public void saveSpreadSheetMLFile(String targetFile)
```


يحفظ البيانات إلى ملف SpreadSheetML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| targetFile | java.lang.String | اسم الملف. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


يحفظ أوراق العمل إلى ملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | الدفق الذي سيُكتب إليه. |

### saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions) {#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)
```


يحفظ أوراق العمل إلى ملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | الدفق الذي سيُكتب إليه. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | خيارات الحفظ. |

### saveToExcelFile(OutputStream stream, int format) {#saveToExcelFile-java.io.OutputStream-int-}
```
public void saveToExcelFile(OutputStream stream, int format)
```


يحفظ أوراق العمل إلى ملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | الدفق الذي سيُكتب إليه. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). تنسيق الملف (Excel2003, Excel2007, CSV, SpreadsheetML) |

### saveToExcelFile(String targetFile) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String targetFile)
```


يحفظ أوراق العمل إلى ملف إكسل بتنسيق Excel 2003.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| targetFile | java.lang.String | اسم الملف الهدف للكتابة إليه. |

### saveToExcelFile(String targetFile, GridSaveOptions saveOptions) {#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(String targetFile, GridSaveOptions saveOptions)
```


يحفظ أوراق العمل إلى ملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| targetFile | java.lang.String | اسم الملف الهدف للكتابة إليه. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | خيارات الحفظ. |

### saveToExcelFile(String targetFile, int format) {#saveToExcelFile-java.lang.String-int-}
```
public void saveToExcelFile(String targetFile, int format)
```


يحفظ أوراق العمل إلى ملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| targetFile | java.lang.String | اسم الملف الهدف للكتابة إليه. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). تنسيق الملف (Excel2003, Excel2007, CSV, SpreadsheetML) |

### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```


يضبط مسار الويب لملفات السكريبت/الصورة الخاصة بالتحكم. على سبيل المثال: "http://localhost/acw\_client". يمكنك أيضًا ضبط هذه القيمة في ملف web.config. أضف هذا القسم إلى قسم `<configuration>`:
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```


يضبط عنوان URL للويب لملف اللغة الخاص بالتحكم. على سبيل المثال: "/acw\_client/lang\_en.js".
بشكل افتراضي، يتم استخدام ملف إنجليزي مدمج.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```


يضبط الخلية النشطة في الورقة الحالية. تم تغييره ليكون قابلًا للكتابة منذ الإصدار 1.9.0.1.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


يحدد لون الخلفية للخلية النشطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


يحدد لون الخلية النشطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


يحدد لون الخلفية لرأس الصف/العمود النشط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


يحدد لون رأس الصف/العمود النشط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


يضبط فهرس الورقة النشطة. يساوي WebWorksheets.ActiveSheetIndex.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```


يحدد نمط التبويب النشط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```


يضبط ما إذا كان يتم تحديث صورة المخطط أثناء تحديث قيمة الخلية. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


يضبط BackColor في WebControl

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


يضبط BorderColor في WebControl

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


يضبط BorderStyle في WebControl

انظر [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


يضبط BorderWidth في WebControl

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```


يضبط نمط الشريط السفلي للتحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


يضبط ما إذا كان سيتم حساب الصيغة بعد تغير قيمة الخلية أو بعد استيراد الملف. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


يضبط CssClass في WebControl

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```


يضبط فهرس الصفحة الحالية في وضع التصفح.

**Remarks**

عند تشغيل وضع الصفحات، سيعرض التحكم PageSize صفوف من البيانات مرة واحدة، ويعرض عنصر التحكم لتحديد الصفحة في شريط التبويب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```


يمثل محرك حساب مخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine) |  |

### setCustomStyle(InputStream stream) {#setCustomStyle-java.io.InputStream-}
```
public void setCustomStyle(InputStream stream)
```


يضبط ملف النمط المخصص من التدفق بما في ذلك تدفق ملف القرص أو تدفق الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق الملف، بما في ذلك تدفق ملف القرص أو تدفق الذاكرة. |

### setCustomStyleFileName(String value) {#setCustomStyleFileName-java.lang.String-}
```
public void setCustomStyleFileName(String value)
```


يضبط اسم ملف النمط المخصص.

**Remarks**

ملف النمط المخصص هو ملف XML. عند تعيين اسم الملف، سيتم تحميل الملف فورًا. هنا محتوى "النمط المسبق القياسي" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


يحصل على / يضبط DPI للجهاز.

**Remarks**

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


يضبط اسم الخط الافتراضي للعنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


يضبط حجم الخط الافتراضي للتحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```


يضبط لون خط الشبكة الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```


يضبط ما إذا كان يتم عرض النصائح. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```


يضبط وضع التحرير للتحكم.

**Remarks**

عند تعيينه إلى true، خلايا التحكم قابلة للتحرير، ويتم عرض أيقونتي "save" و "undo". عند تعيينه إلى false، تكون خلايا التحكم للقراءة فقط، ولا يتم عرض أيقونتي "save" و "undo".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```


يضبط ما إذا كان يتم استخدام استدعاء AJAX. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```


يضبط ما إذا كان يتم تحميل بيانات الخلايا بطريقة غير متزامنة، يُنصح بتطبيق ذلك على ورقة واحدة تحتوي على أكثر من 10000 خلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```


يضبط ما إذا كان يتم تمكين عمليات الأعمدة على جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم استخدام قائمة النقر بزر الفأرة الأيمن لإضافة/إزالة الأعمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```


يضبط ما إذا كان يتم تمكين عمليات التجميد على جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم استخدام قائمة النقر بزر الفأرة الأيمن لتجميد/إلغاء تجميد الألواح.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```


يضبط ما إذا كان يتم تمكين عمليات الدمج على جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم استخدام قائمة النقر بزر الفأرة الأيمن لدمج/فصل الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```


يحدد ما إذا كان سيتم تمكين تعديل حجم الأعمدة والصفوف من جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم تغيير حجم العمود والصف على جانب العميل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```


يحدد ما إذا كان سيتم تمكين عمليات الصف من جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم استخدام قائمة النقر بزر الفأرة الأيمن لإضافة/إزالة الصفوف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```


يحدد ما إذا كان سيتم تمكين حدث النقر المزدوج من جانب العميل.

**Remarks**

عند تعيينه إلى true، سيتلقى التحكم أحداث النقر المزدوج على جانب العميل ويمكنك معالجة هذه الأحداث على جانب الخادم. وإلا سيتجاهل التحكم أي أحداث نقر مزدوج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```


يحدد ما إذا كان سيتم تطبيق تأثير الضوء المعدني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```


يحدد ما إذا كان سيتم تمكين وضع ترقيم الصفحات للعنصر.

**Remarks**

عند تعيينه إلى true، سيعرض التحكم عدد صفوف PageSize من البيانات مرة واحدة، ويعرض عنصر التحكم لاختيار الصفحة في شريط التبويب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```


يحدد ما إذا كان سيتم تمكين مربع حوار النمط من جانب العميل.

**Remarks**

عند تعيينه إلى true، يمكن للمستخدم استخدام مربع حوار النمط لتعيين نمط الخلية عن طريق اختيار "Format Cell..." من القائمة المنبثقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


يضبط Enabled في WebControl

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```


يحدد ما إذا كان سيتم تمكين الترقيم بعد تصفية البيانات، سيصبح ساريًا عندما تكون EnablePaging صحيحة.

**Remarks**

عند تعيينه إلى true، سيقوم التحكم بالترقيم بناءً على البيانات المفلترة، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```


يحدد ما إذا كان سيتم فرض التحقق من الصحة من جانب العميل.

**Remarks**

عند تعيينه إلى true، لن يتم إرسال البيانات إلى الخادم حتى تكون جميع حقول الإدخال صالحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


يضبط ForeColor في WebControl

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```


يحدد نمط الإطار للعنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```


يحدد ما إذا كان GridWeb سيقوم بعملية الحفظ الافتراضية، القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```


يحدد ارتفاع (System.Web.UI.WebControl.Unit) شريط الرأس العلوي للعنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```


يحدد نمط شريط الرأس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```


يحدد نمط شريط الرأس للعنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```


يحدد عرض (System.Web.UI.WebControl.Unit) شريط الرأس الأيسر للعنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


يحدد ارتفاع (System.Web.UI.WebControl.Unit) للعنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```


يضبط ما إذا كان GridWeb يتجاهل إظهار الصفوف أو الأعمدة التي لا تحتوي على قيم خلايا ولكنها لا تزال مُنسقة. إذا تم تعيينه إلى true، سيتحسن الأداء. القيمة الافتراضية هي false، مما يعني أنه إذا كان الصف/العمود المتتالي الأخير لا يحتوي على قيم خلايا ولكنه مُنسق، فسنظل نعرضه. هذا الخيار صالح فقط عندما EnableAsync يكون false. لا يؤثر هذا الخيار عندما EnableAsync يكون true، مما يعني أن GridWeb سيعرض جميع الصفوف/الأعمدة ذات النمط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLoadOptions(GridLoadOptions value) {#setLoadOptions-com.aspose.gridweb.GridLoadOptions-}
```
public void setLoadOptions(GridLoadOptions value)
```


يمثل خيارات التحميل لـ GridWeb.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridLoadOptions](../../com.aspose.gridweb/gridloadoptions) |  |

### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```


يضبط الحد الأقصى لمؤشر عرض العمود (مبني على الصفر) للورقة الويب. يستخدم التحكم القيمة الأكبر بين MaxColumn والحد الأقصى للعمود في بيانات الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```


يضبط الحد الأقصى لمؤشر عرض الصف (مبني على الصفر) للورقة الويب. يستخدم التحكم القيمة الأكبر بين MaxRow والحد الأقصى للصف في بيانات الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```


يحدد الرسالة للشبكة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```


يضبط الحد الأدنى لمؤشر عرض العمود (مبني على الصفر) للورقة الويب. يستخدم التحكم القيمة الأصغر بين MinColumn والحد الأدنى للعمود في بيانات الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```


يضبط الحد الأدنى لمؤشر عرض الصف (مبني على الصفر) للورقة الويب. يستخدم التحكم القيمة الأصغر بين MinRow والحد الأدنى للصف في بيانات الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```


يحدد ما إذا كان سيتم إظهار صفوف المجموعات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```


يحدد قيمة تشير إلى ما إذا كان شريط التمرير الأفقي مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```


يحدد ما إذا كان سيتم إظهار شريط التمرير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```


يحدد قيمة تشير إلى ما إذا كان شريط التمرير العمودي مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```


يضبط اسم الدالة على جانب العميل التي سيتم استدعاؤها عند انتهاء ajaxcall. يجب إعلان الدالة على العميل كما يلي:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```


يضبط اسم الدالة على جانب العميل التي سيتم استدعاؤها عندما تفشل عملية التحقق من صحة الخلية. يجب إعلان الدالة على العميل كما يلي:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```


يضبط الدالة على جانب العميل التي سيتم استدعاؤها عند تحديد خلية. يجب إعلان الدالة على العميل كما يلي:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```


يضبط الدالة على جانب العميل التي سيتم استدعاؤها عند تحديد خلية. يجب إعلان الدالة على العميل كما يلي:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```


يضبط الدالة على جانب العميل التي سيتم استدعاؤها عند إلغاء تحديد خلية. يجب إعلان الدالة على العميل كما يلي:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```


يضبط اسم الدالة على جانب العميل التي سيتم استدعاؤها عند تحديث قيمة الخلية. يجب إعلان الدالة على العميل كما يلي:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```


يضبط الدالة على جانب العميل التي سيتم استدعاؤها عند عرض قائمة السياق. يجب إعلان الدالة على العميل كما يلي:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```


يضبط الدالة على جانب العميل التي سيتم استدعاؤها عند النقر المزدوج على خلية. يجب إعلان الدالة على العميل كما يلي:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```


يضبط الدالة على جانب العميل التي سيتم استدعاؤها عند النقر المزدوج على صف. يجب إعلان الدالة على العميل كما يلي:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```


يضبط اسم الدالة على جانب العميل التي سيتم استدعاؤها عند تهيئة الشبكة. يجب إعلان الدالة على العميل كما يلي:
function MyOnGridInit(grid)
\{
alert("The grid is initialized: " + grid.id);
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```


يضبط الدالة على جانب العميل التي سيتم استدعاؤها بعد تغيير فهرس الصفحة. سيتأثر فقط عندما EnablePaging يكون true. يجب إعلان الدالة على العميل كما يلي:
function MyOnPageChange(index)
\{
console.log("current page is:"+index);
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```


يضبط الدالة على جانب العميل التي تُستدعى قبل إرسال الصفحة من جانب العميل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```


يضبط الدالة على جانب العميل التي سيتم استدعاؤها عند تحديد شكل. يجب إعلان الدالة على العميل كما يلي:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```


يضبط الدالة على جانب العميل التي سيتم استدعاؤها قبل إرسال التحكم من جانب العميل. يجب إعلان الدالة على العميل كما يلي:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
المتغير arg هو معامل الإرسال، يحتوي على الأمر الذي سيُرسل إلى الخادم. المتغير cancelEdit هو قيمة منطقية تشير إلى ما إذا كان التحكم قد تخلص من إدخال المستخدم قبل الإرسال. سيستمر التحكم في الإرسال إذا أعادت الدالة القيمة true.
ملاحظة: يمكنك استخدام المؤشر "this" في الدالة على الجانب العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


يضبط ما إذا كان يتم ضبط الصفوف التي ارتفاعها غير مخصص فقط، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```


يضبط حجم الصفحة في وضع التقسيم.

**Remarks**

عند تشغيل وضع الصفحات، سيعرض التحكم PageSize صفوف من البيانات مرة واحدة، ويعرض عنصر التحكم لتحديد الصفحة في شريط التبويب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```


يضبط مسار تخزين الصور لدفتر العمل، جميع الأشكال والصور ستُخزن في هذا الدليل، المسار الافتراضي هو acwcache داخل دليل قاعدة التطبيق الحالي، يحتاج المستخدمون إلى تنفيذ خدمة جدولة لتنظيف الملفات التي انتهى وقت جلسةها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


يضبط النمط المسبق.

انظر [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```


يضبط ما إذا كان سيتم تحديث قيمة التحقق بعد تغيير قيمة الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```


يضبط ما إذا كان الصف المخفي يُعرض في GridControl، القيمة الافتراضية هي false. إذا كنت بحاجة إلى إظهار الصف المخفي لاحقًا، يجب تعيينه إلى true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRowHeightForCSV(double value) {#setRowHeightForCSV-double-}
```
public void setRowHeightForCSV(double value)
```


يضبط قيمة ارتفاع الصف بالنقطة لملف csv، القيمة الافتراضية هي 14.5.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```


يحدد لون زر السهم لشريط التمرير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```


يحدد لون شريط التمرير للعنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


يحدد لون خلفية الخلايا المحددة في نطاق التحديد المتعدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


يحدد لون الخلايا المحددة في نطاق التحديد المتعدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```


يضبط مسار تخزين ذاكرة التخزين المؤقت للجلسة عندما يكون وضع الجلسة File أو ViewState، إلخ: gridweb.SessionStorePath="c:/mytempdir/session"؛ ثم سيُخزن بيانات الجلسة في c:/mytempdir/session.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


يمثل إعدادات المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |

### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```


يضبط ما إذا كان سيتم إظهار زر إضافة ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```


يحدد ما إذا كان سيتم عرض شريط الأوامر (يشمل شريط الأوامر وشريط التبويب) في أسفل العنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```


ما إذا كان Gridweb يعرض شريط أدوات مربع التحرير كما في MS-EXCEL. إذا تم التفعيل، سيظهر مربع تحرير للخلية الحالية في Gridweb. عند تفعيل هذه الميزة، نحتاج إلى استيراد مكتبة jquery js في ملفات aspx الخاصة بك لدعم هذه الميزة الجديدة. أي نسخة حديثة من jquery تعمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```


يحدد ما إذا كان سيتم عرض شريط الأوامر (يشمل شريط الأوامر وشريط التبويب) في أعلى العنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```


يضبط ما إذا كان سيتم إظهار قائمة السياق. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```


يضبط ما إذا كان سيتم إظهار خطوط الشبكة الافتراضية للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```


يضبط ما إذا كان سيتم إظهار شريط العنوان

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```


يحدد ما إذا كان سيتم عرض مربع حوار التحميل أثناء الإرسال إلى الخادم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```


يحدد الموضع الأيسر والعلوي (بالبكسل) لعرض مربع حوار التحميل أثناء الإرسال إلى الخادم، إلخ. 100,200 يعني أن موضع مربع حوار التحميل الأيسر والعلوي هو 100px,200px.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```


يضبط ما إذا كان سيتم عرض زر الحفظ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```


يضبط ما إذا كان سيتم عرض زر الإرسال.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```


يضبط ما إذا كان سيتم عرض شريط علامات التبويب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```


يضبط ما إذا كان زر تنقل علامات التبويب معروضًا، القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```


يضبط ما إذا كان سيتم عرض زر التراجع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```


يحدد ما إذا كان سيتم لف المحتوى داخل امتداد الخلية، القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTabIndex(short value) {#setTabIndex-short-}
```
public void setTabIndex(short value)
```


يضبط TabIndex في WebControl

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | short |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```


يضبط نمط شريط علامات التبويب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


يضبط ToolTip في WebControl

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```


يضبط ما إذا كان GridWeb يستخدم ارتفاع صفحة العميل كارتفاع للعنصر، مناسب عندما يتم تعيين Height=\"100%\", القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```


يضبط موضع شريط التمرير في لوحة عرض الشبكة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```


يضبط موضع شريط التمرير في لوحة عرض الشبكة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```


يضبط نمط لوحة عرض البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


يضبط عرض (System.Web.UI.WebControl.Unit) للعنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```


يضبط ما إذا كان سيتم استخدام نمط XHTML، القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

