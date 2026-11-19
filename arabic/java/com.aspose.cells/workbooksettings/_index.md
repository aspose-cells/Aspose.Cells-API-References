---
title: "WorkbookSettings"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع إعدادات المصنف."
type: docs
url: /ar/java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

يمثل جميع إعدادات المصنف.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorkbookSettings settings = workbook.getSettings();
 
         //do your business
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [dispose()](#dispose--) | يطلق الموارد. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | يحصل على مؤلف الملف. |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | يحدد قيمة منطقية تشير إلى أن التطبيق يضغط الصور تلقائيًا في دفتر العمل. |
| [getAutoRecover()](#getAutoRecover--) | يشير إلى ما إذا كان الملف محددًا للاستعادة التلقائية. |
| [getBuildVersion()](#getBuildVersion--) | يحدد الإصدار العام المتدرج للتطبيق. |
| [getCheckCompatibility()](#getCheckCompatibility--) | يشير إلى ما إذا كان يتم فحص التوافق مع الإصدارات السابقة عند حفظ دفتر العمل. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | يشير إلى ما إذا كان يتم فحص تنسيق الأرقام المخصص عند تعيين Style.Custom. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | يحدد إصدار OOXML للمستند الناتج. |
| [getCrashSave()](#getCrashSave--) | يشير إلى ما إذا كان التطبيق قد حفظ ملف دفتر العمل آخر مرة بعد تعطل. |
| [getDataExtractLoad()](#getDataExtractLoad--) | يشير إلى ما إذا كان التطبيق قد فتح دفتر العمل آخر مرة لاستعادة البيانات. |
| [getDate1904()](#getDate1904--) | يحصل على قيمة تمثل ما إذا كان دفتر العمل يستخدم نظام التاريخ 1904. |
| [getDefaultImageResolution()](#getDefaultImageResolution--) | يحصل على الدقة الافتراضية للصورة. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | يحصل على الإعدادات للقيم الافتراضية للخصائص المتعلقة بالنمط لهذا دفتر العمل. |
| [getDiscardImageEditData()](#getDiscardImageEditData--) | يشير إلى ما إذا كان يتم تجاهل بيانات تحرير الصورة. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | يشير إلى ما إذا كان وكيفية عرض الكائنات في دفتر العمل. |
| [getEnableMacros()](#getEnableMacros--) | تمكين الماكرو؛ |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | يحصل على أول علامة ورقة عمل مرئية. |
| [getFormulaSettings()](#getFormulaSettings--) | يحصل على الإعدادات للميزات المتعلقة بالمعادلات. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | يحصل على إعدادات العولمة. |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | يحصل على ما إذا كان يتم إخفاء قائمة الحقول لجدول Pivot. |
| [getLanguageCode()](#getLanguageCode--) | يحصل على لغة واجهة المستخدم لإصدار دفتر العمل بناءً على رمز البلد الذي تم حفظ الملف به. |
| [getLocale()](#getLocale--) | يحصل على الإعداد الإقليمي المستخدم في دفتر العمل هذا. |
| [getMaxColumn()](#getMaxColumn--) | يحصل على الحد الأقصى لمؤشر العمود، بدءًا من الصفر. |
| [getMaxRow()](#getMaxRow--) | يحصل على الحد الأقصى لمؤشر الصف، بدءًا من الصفر. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | يحصل على الحد الأقصى لرقم الصف للمعادلة المشتركة. |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--) | يحصل على الحد الأقصى للعناصر الفريدة لكل حقل |
| [getMemorySetting()](#getMemorySetting--) | يحصل على خيارات استخدام الذاكرة. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | يحصل على الفاصل العشري لتنسيق/تحليل القيم الرقمية. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | يحصل على الحرف الذي يفصل مجموعات الأرقام إلى يسار الفاصل العشري في القيم الرقمية. |
| [getPaperSize()](#getPaperSize--) | يحصل على حجم الورق الافتراضي للطباعة. |
| [getPassword()](#getPassword--) | يمثل كلمة مرور تشفير ملف المصنف. |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--) | يشير إلى ما إذا كانت خصائص نقاط البيانات وملصقات البيانات في جميع المخططات في هذا المصنف تتبع مرجعها. |
| [getProtectionType()](#getProtectionType--) | يحصل على نوع الحماية للمصنف. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | يشير إلى ما إذا كان ضبط خاصية [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) عند إدخال قيمة النص (التي تبدأ بعلامة اقتباس مفردة) إلى الخلية |
| [getRegion()](#getRegion--) | يحصل على الإعدادات الإقليمية للمصنف. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | صحيح إذا كان يمكن إزالة المعلومات الشخصية من المصنف المحدد. |
| [getRepairLoad()](#getRepairLoad--) | يشير إلى ما إذا كان التطبيق قد فتح المصنف في وضع الأمان أو الإصلاح آخر مرة. |
| [getResourceProvider()](#getResourceProvider--) | يحصل على موفر الدفق للموارد الخارجية، مثل تحميل بيانات الصورة للرسمة من النوع "LinkToFile". |
| [getShapeDisplayType()](#getShapeDisplayType--) | يحصل على طريقة عرض التطبيق للأشكال في هذا المصنف. |
| [getShared()](#getShared--) | يحصل على قيمة تشير إلى ما إذا كان المصنف مشتركًا. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | عرض شريط علامات تبويب ورقة العمل (بـ 1/1000 من عرض النافذة). |
| [getShowTabs()](#getShowTabs--) | يحصل على قيمة ما إذا كانت علامات تبويب المصنف معروضة. |
| [getSignificantDigits()](#getSignificantDigits--) | يحصل على عدد الأرقام ذات الدقة. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | يحصل على نوع الأرقام ذات الدقة لإخراج القيم الرقمية في هذا المصنف. |
| [getSmartTagOptions()](#getSmartTagOptions--) | يحصل على خيارات العلامة الذكية. |
| [getStreamProvider()](#getStreamProvider--) | يحصل على موفر الدفق للموارد الخارجية. |
| [getThemeFont(int type)](#getThemeFont-int-) | يحصل على اسم خط السمة الافتراضي. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | يشير إلى ما إذا كان يتم تحديث حدود الخلايا المجاورة. |
| [getUpdateLinksType()](#getUpdateLinksType--) | يحصل على طريقة تحديث الروابط الخارجية عند فتح المصنف. |
| [getWarningCallback()](#getWarningCallback--) | يحصل على رد النداء للتحذير. |
| [getWindowHeight()](#getWindowHeight--) | ارتفاع النافذة، بوحدة النقطة. |
| [getWindowHeightCM()](#getWindowHeightCM--) | ارتفاع النافذة، بوحدة السنتيمتر. |
| [getWindowHeightInch()](#getWindowHeightInch--) | ارتفاع النافذة، بوحدة البوصة. |
| [getWindowLeft()](#getWindowLeft--) | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة، بوحدة النقطة. |
| [getWindowLeftCM()](#getWindowLeftCM--) | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. |
| [getWindowLeftInch()](#getWindowLeftInch--) | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. |
| [getWindowTop()](#getWindowTop--) | المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة النقطة. |
| [getWindowTopCM()](#getWindowTopCM--) | المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة السنتيمتر. |
| [getWindowTopInch()](#getWindowTopInch--) | المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة البوصة. |
| [getWindowWidth()](#getWindowWidth--) | عرض النافذة، بوحدة النقطة. |
| [getWindowWidthCM()](#getWindowWidthCM--) | عرض النافذة، بوحدة السنتيمتر. |
| [getWindowWidthInch()](#getWindowWidthInch--) | عرض النافذة، بوحدة البوصة. |
| [getWpsCompatibility()](#getWpsCompatibility--) | يشير إلى ما إذا كان يجب أن يكون متوافقًا مع WPS. |
| [getWriteProtection()](#getWriteProtection--) | يوفر الوصول إلى خيارات حماية الكتابة في دفتر العمل. |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | يشير إلى ما إذا كان سيتم تشفير دفتر العمل باستخدام كلمة مرور افتراضية إذا تم قفل الهيكل والنوافذ لدفتر العمل. |
| [isEncrypted()](#isEncrypted--) | يحصل على قيمة تشير إلى ما إذا كانت كلمة المرور مطلوبة لفتح هذا دفتر العمل. |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | يحصل على قيمة تشير إلى ما إذا كان جدول البيانات المُنشأ سيحتوي على شريط تمرير أفقي. |
| [isHidden()](#isHidden--) | يشير إلى ما إذا كان هذا دفتر العمل مخفيًا. |
| [isMinimized()](#isMinimized--) | يمثل ما إذا كان جدول البيانات المُنشأ سيفتح مصغرًا. |
| [isProtected()](#isProtected--) | يحصل على قيمة تشير إلى ما إذا كان الهيكل أو نافذة دفتر العمل محميًا. |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | يحصل على قيمة تشير إلى ما إذا كان جدول البيانات المُنشأ سيحتوي على شريط تمرير عمودي. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | يضبط مؤلف الملف. |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | يحدد قيمة منطقية تشير إلى أن التطبيق يضغط الصور تلقائيًا في دفتر العمل. |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | يشير إلى ما إذا كان الملف محددًا للاستعادة التلقائية. |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | يحدد الإصدار العام المتدرج للتطبيق. |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | يشير إلى ما إذا كان يتم فحص التوافق مع الإصدارات السابقة عند حفظ دفتر العمل. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | يشير إلى ما إذا كان يتم فحص تنسيق الأرقام المخصص عند تعيين Style.Custom. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setCompliance(int value)](#setCompliance-int-) | يحدد إصدار OOXML للمستند الناتج. |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | يشير إلى ما إذا كان التطبيق قد حفظ ملف دفتر العمل آخر مرة بعد تعطل. |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | يشير إلى ما إذا كان التطبيق قد فتح دفتر العمل آخر مرة لاستعادة البيانات. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | يضبط قيمة تمثل ما إذا كان دفتر العمل يستخدم نظام التاريخ 1904. |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | يشير إلى ما إذا كان سيتم تشفير دفتر العمل باستخدام كلمة مرور افتراضية إذا تم قفل الهيكل والنوافذ لدفتر العمل. |
| [setDefaultImageResolution(int value)](#setDefaultImageResolution-int-) | يضبط الدقة الافتراضية للصورة. |
| [setDiscardImageEditData(boolean value)](#setDiscardImageEditData-boolean-) | يشير إلى ما إذا كان يتم تجاهل بيانات تحرير الصورة. |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | يشير إلى ما إذا كان وكيفية عرض الكائنات في دفتر العمل. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | تمكين الماكرو؛ |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | يضبط علامة تبويب ورقة العمل الأولى المرئية. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | يضبط إعدادات العولمة. |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | يضبط قيمة تشير إلى ما إذا كان جدول البيانات المُنشأ سيحتوي على شريط تمرير أفقي. |
| [setHidden(boolean value)](#setHidden-boolean-) | يشير إلى ما إذا كان هذا دفتر العمل مخفيًا. |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | يضبط ما إذا كان سيتم إخفاء قائمة الحقول لجدول المحور. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | يضبط لغة واجهة المستخدم لإصدار المصنف بناءً على CountryCode الذي حفظ الملف. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | يضبط اللغة المستخدمة في هذا المصنف. |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | يضبط الحد الأقصى لعدد الصفوف للمعادلة المشتركة. |
| [setMaxUniqueItemsPerField(int value)](#setMaxUniqueItemsPerField-int-) | يضبط الحد الأقصى للعناصر الفريدة لكل حقل |
| [setMemorySetting(int value)](#setMemorySetting-int-) | يضبط خيارات استخدام الذاكرة. |
| [setMinimized(boolean value)](#setMinimized-boolean-) | يمثل ما إذا كان جدول البيانات المُنشأ سيفتح مصغرًا. |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | يضبط الفاصل العشري لتنسيق/تحليل القيم الرقمية. |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | يضبط الحرف الذي يفصل مجموعات الأرقام إلى يسار الفاصل العشري في القيم الرقمية. |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | اضبط نوع اتجاه الطباعة للمصنف بأكمله. |
| [setPaperSize(int value)](#setPaperSize-int-) | يضبط حجم ورق الطباعة الافتراضي. |
| [setPassword(String value)](#setPassword-java.lang.String-) | يمثل كلمة مرور تشفير ملف المصنف. |
| [setPropertiesFollowChartPoint(boolean value)](#setPropertiesFollowChartPoint-boolean-) | يشير إلى ما إذا كانت خصائص نقاط البيانات وملصقات البيانات في جميع المخططات في هذا المصنف تتبع مرجعها. |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | يشير إلى ما إذا كان ضبط خاصية [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) عند إدخال قيمة النص (التي تبدأ بعلامة اقتباس مفردة) إلى الخلية |
| [setRegion(int value)](#setRegion-int-) | يضبط الإعدادات الإقليمية للمصنف. |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | صحيح إذا كان يمكن إزالة المعلومات الشخصية من المصنف المحدد. |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | يشير إلى ما إذا كان التطبيق قد فتح المصنف في وضع الأمان أو الإصلاح آخر مرة. |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | يضبط موفر الدفق للموارد الخارجية، مثل تحميل بيانات الصورة للصور من النوع \"LinkToFile\". |
| [setShapeDisplayType(int value)](#setShapeDisplayType-int-) | يضبط طريقة عرض التطبيق للأشكال في هذا المصنف |
| [setShared(boolean value)](#setShared-boolean-) | يضبط قيمة تشير إلى ما إذا كان المصنف مشتركًا. |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | عرض شريط علامات تبويب ورقة العمل (بـ 1/1000 من عرض النافذة). |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | يضبط قيمة ما إذا كانت علامات تبويب المصنف معروضة. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | يضبط عدد الأرقام ذات الدقة. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | يضبط نوع الأرقام ذات الدقة للخرج القيم الرقمية في هذا المصنف. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | يضبط موفر الدفق للموارد الخارجية. |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | يشير إلى ما إذا كان يتم تحديث حدود الخلايا المجاورة. |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | يضبط طريقة تحديث الروابط الخارجية عند فتح المصنف. |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | يضبط قيمة تشير إلى ما إذا كان جدول البيانات المُنشأ سيحتوي على شريط تمرير عمودي. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | يضبط رد النداء للتحذير. |
| [setWindowHeight(double value)](#setWindowHeight-double-) | ارتفاع النافذة، بوحدة النقطة. |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | ارتفاع النافذة، بوحدة السنتيمتر. |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | ارتفاع النافذة، بوحدة البوصة. |
| [setWindowLeft(double value)](#setWindowLeft-double-) | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة، بوحدة النقطة. |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. |
| [setWindowTop(double value)](#setWindowTop-double-) | المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة النقطة. |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة السنتيمتر. |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة البوصة. |
| [setWindowWidth(double value)](#setWindowWidth-double-) | عرض النافذة، بوحدة النقطة. |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | عرض النافذة، بوحدة السنتيمتر. |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | عرض النافذة، بوحدة البوصة. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | يشير إلى ما إذا كان يجب أن يكون متوافقًا مع WPS. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### dispose() {#dispose--}
```
public void dispose()
```


يطلق الموارد.

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


يحصل على مؤلف الملف.

**Remarks**

لم يتم تعيينه، تحقق أولاً من [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--)، ثم تحقق من مستخدم البيئة.

**Returns:**
java.lang.String
### getAutoCompressPictures() {#getAutoCompressPictures--}
```
public boolean getAutoCompressPictures()
```


يحدد قيمة منطقية تشير إلى أن التطبيق يضغط الصور تلقائيًا في دفتر العمل.

**Returns:**
boolean
### getAutoRecover() {#getAutoRecover--}
```
public boolean getAutoRecover()
```


يشير إلى ما إذا كان الملف محددًا للاستعادة التلقائية.

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


يحدد الإصدار العام المتدرج للتطبيق.

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


يشير إلى ما إذا كان يتم فحص التوافق مع الإصدارات السابقة عند حفظ دفتر العمل.

**Remarks**

القيمة الافتراضية هي true. فقط لملفات Excel97-2003 xls أو xlt.

**Returns:**
boolean
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


يشير إلى ما إذا كان يتم فحص تنسيق الأرقام المخصص عند تعيين Style.Custom.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا عبر Cell.PutValue(string)، إذا كانت هذه الخاصية true ستحصل على استثناء. إذا كانت false، سنقبل قيمة السلسلة التي أدخلتها كقيمة للخلية بحيث يمكنك لاحقًا إخراج القيمة الكاملة للملفات الأخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


يحدد إصدار OOXML للمستند الناتج. القيمة الافتراضية هي Ecma376\_2006.

انظر [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

فقط لملفات .xlsx.

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


يشير إلى ما إذا كان التطبيق قد حفظ ملف دفتر العمل آخر مرة بعد تعطل.

**Returns:**
boolean
### getDataExtractLoad() {#getDataExtractLoad--}
```
public boolean getDataExtractLoad()
```


يشير إلى ما إذا كان التطبيق قد فتح دفتر العمل آخر مرة لاستعادة البيانات.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


يحصل على قيمة تمثل ما إذا كان دفتر العمل يستخدم نظام التاريخ 1904.

**Returns:**
boolean
### getDefaultImageResolution() {#getDefaultImageResolution--}
```
public int getDefaultImageResolution()
```


يحصل على الدقة الافتراضية للصورة.

**Returns:**
int
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


يحصل على الإعدادات للقيم الافتراضية للخصائص المتعلقة بالنمط لهذا دفتر العمل.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDiscardImageEditData() {#getDiscardImageEditData--}
```
public boolean getDiscardImageEditData()
```


يشير إلى ما إذا كان يتم تجاهل بيانات تحرير الصورة.

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


يشير إلى ما إذا كان وكيفية عرض الكائنات في دفتر العمل.

انظر [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


تمكين الماكرو؛

**Remarks**

الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في مصنف.

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


يحصل على أول علامة ورقة عمل مرئية.

**Returns:**
int
### getFormulaSettings() {#getFormulaSettings--}
```
public FormulaSettings getFormulaSettings()
```


يحصل على الإعدادات للميزات المتعلقة بالمعادلات.

**Returns:**
[FormulaSettings](../../com.aspose.cells/formulasettings)
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public GlobalizationSettings getGlobalizationSettings()
```


يحصل على إعدادات العولمة.

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


يحصل على ما إذا كان يتم إخفاء قائمة الحقول لجدول Pivot.

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


يحصل على لغة واجهة المستخدم لإصدار دفتر العمل بناءً على رمز البلد الذي تم حفظ الملف به.

انظر [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


يحصل على الإعداد الإقليمي المستخدم في دفتر العمل هذا.

**Remarks**

يرجع null إذا لم يتم تعيين لا Locale ولا [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--).

**Returns:**
java.util.Locale
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


يحصل على الحد الأقصى لمؤشر العمود، بدءًا من الصفر.

**Remarks**

يعيد 255 إذا كان تنسيق الملف هو Excel97-2003؛

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


يحصل على الحد الأقصى لمؤشر الصف، بدءًا من الصفر.

**Remarks**

يعيد 65535 إذا كان تنسيق الملف هو Excel97-2003؛

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


يحصل على الحد الأقصى لرقم الصف للمعادلة المشتركة.

**Remarks**

إذا كان الرقم كبيرًا جدًا، فإن الفلتر التلقائي يعمل ببطء شديد في MS Excel 2013.

**Returns:**
int
### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}
```
public int getMaxUniqueItemsPerField()
```


يحصل على الحد الأقصى للعناصر الفريدة لكل حقل

**Remarks**

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


يحصل على خيارات استخدام الذاكرة. سيتم اتخاذ الخيار الجديد كخيار افتراضي للأوراق التي تم إنشاؤها حديثًا ولكنه لا يؤثر على الأوراق الموجودة.

انظر [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

لمزيد من التفاصيل حول وضع الذاكرة، يرجى الاطلاع على [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


يحصل على الفاصل العشري لتنسيق/تحليل القيم الرقمية. الافتراضي هو الفاصل العشري للمنطقة الحالية.

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


يحصل على الحرف الذي يفصل مجموعات الأرقام إلى يسار الفاصل العشري في القيم الرقمية. الافتراضي هو فاصل المجموعات للمنطقة الحالية.

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


يحصل على حجم الورق الافتراضي للطباعة.

انظر [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

إذا لم يكن هناك إعداد لحجم الورق، سيستخدم MS Excel إعداد الطابعة الافتراضي.

**Returns:**
int
### getPassword() {#getPassword--}
```
public String getPassword()
```


يمثل كلمة مرور تشفير ملف المصنف.

**Returns:**
java.lang.String
### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}
```
public boolean getPropertiesFollowChartPoint()
```


يشير إلى ما إذا كانت خصائص نقاط البيانات وملصقات البيانات في جميع المخططات في هذا المصنف تتبع مرجعها.

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


يحصل على نوع الحماية للمصنف.

انظر [ProtectionType](../../com.aspose.cells/protectiontype).

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


يشير إلى ما إذا كان ضبط خاصية [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) عند إدخال قيمة النص (التي تبدأ بعلامة اقتباس مفردة) إلى الخلية

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


يحصل على الإعدادات الإقليمية للمصنف.

انظر [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. الإعدادات الإقليمية التي يستخدمها مكوّن Aspose.Cells لدفتر عمل تم تحميله من ملف قالب: i). بالنسبة لملف XLS، هناك حقول معرفة للإعدادات الإقليمية وتقوم MS Excel بحفظ بيانات الإعدادات الإقليمية في الملف عند حفظ ملف XLS. لذلك، نستخدم المنطقة المحفوظة في ملف القالب للدفتر. إذا لم ترغب في استخدام المنطقة المحفوظة في ملف XLS، يرجى إعادة تعيينها إلى القيمة المتوقعة (مثل CountryCode.Default) بعد تحميل ملف القالب. كما أننا نحفظ القيمة المحددة من قبل المستخدم (باستخدام هذه الطريقة) في الملف أيضًا عند حفظ ملف XLS. ii). بالنسبة لتنسيقات الملفات الأخرى، مثل XLSX، XLSB... إلخ، لا توجد حقل معرف للإعدادات الإقليمية في مواصفات تنسيق الملف. لذلك، نستخدم الإعدادات الإقليمية لبيئة التطبيق للدفتر. ولا يمكن الاحتفاظ بالقيمة المحددة من قبل المستخدم (باستخدام هذه الطريقة) للملفات المولدة بتلك التنسيقات. 2. لتأثير العرض في MS Excel: الإعدادات الإقليمية المطبقة هنا يمكن أن تؤثر فقط أثناء التشغيل مع مكوّن Aspose.Cells وليس عند عرض الملف المولد باستخدام MS Excel. حتى بالنسبة لملف XLS المولد الذي تم حفظ بيانات الإعدادات الإقليمية فيه، عند عرضه/تحريره باستخدام MS Excel، تكون المنطقة المستخدمة لتنسيق القيم بواسطة MS Excel دائمًا هي الإعدادات الإقليمية الافتراضية للبيئة التي يعمل فيها MS Excel، وليس تلك المحفوظة في الملف. هذا سلوك MS Excel ولا يمكن تغييره عبر الشيفرة.

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


صحيح إذا كان يمكن إزالة المعلومات الشخصية من المصنف المحدد.

**Remarks**

**Returns:**
boolean
### getRepairLoad() {#getRepairLoad--}
```
public boolean getRepairLoad()
```


يشير إلى ما إذا كان التطبيق قد فتح المصنف في وضع الأمان أو الإصلاح آخر مرة.

**Returns:**
boolean
### getResourceProvider() {#getResourceProvider--}
```
public IStreamProvider getResourceProvider()
```


يحصل على موفر الدفق للموارد الخارجية، مثل تحميل بيانات الصورة للرسمة من النوع "LinkToFile".

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShapeDisplayType() {#getShapeDisplayType--}
```
public int getShapeDisplayType()
```


يحصل على طريقة عرض التطبيق للأشكال في هذا المصنف.

انظر [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Returns:**
int
### getShared() {#getShared--}
```
public boolean getShared()
```


يحصل على قيمة تشير إلى ما إذا كان المصنف مشتركًا.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getSheetTabBarWidth() {#getSheetTabBarWidth--}
```
public int getSheetTabBarWidth()
```


عرض شريط علامات تبويب ورقة العمل (بـ 1/1000 من عرض النافذة).

**Returns:**
int
### getShowTabs() {#getShowTabs--}
```
public boolean getShowTabs()
```


يحصل على قيمة ما إذا كانت علامات تبويب المصنف معروضة.

**Remarks**

القيمة الافتراضية هي true.

**Example**

الكود التالي يخفي Sheet Tabs و Tab Scrolling Buttons لجدول البيانات.

```
         // Hide the spreadsheet tabs.
         workbook.getSettings().setShowTabs(false);
```

**Returns:**
boolean
### getSignificantDigits() {#getSignificantDigits--}
```
public int getSignificantDigits()
```


يحصل على عدد الأرقام المهمة. القيمة الافتراضية هي [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

يمكن أن يكون فقط 15 أو 17 الآن. ملاحظة: هذا العضو أصبح مهجورًا الآن. بدلاً من ذلك، يرجى استخدام [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public int getSignificantDigitsType()
```


يحصل على نوع الأرقام المهمة لإخراج القيم الرقمية في هذا الدفتر. القيمة الافتراضية هي [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

انظر [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getSmartTagOptions() {#getSmartTagOptions--}
```
public SmartTagOptions getSmartTagOptions()
```


يحصل على خيارات العلامة الذكية.

**Returns:**
[SmartTagOptions](../../com.aspose.cells/smarttagoptions)
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


يحصل على موفر الدفق للموارد الخارجية.

**Remarks**

ملاحظة: هذا العضو أصبح مهجورًا الآن. بدلاً من ذلك، يرجى استخدام خاصية ResourceProvider. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getThemeFont(int type) {#getThemeFont-int-}
```
public String getThemeFont(int type)
```


يحصل على اسم خط السمة الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). نوع المخطط للخط. |

**Returns:**
java.lang.String -
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


يشير إلى ما إذا كان يتم تحديث حدود الخلايا المجاورة.

**Remarks**

القيمة الافتراضية هي false. على سبيل المثال: إذا تم تحديث الحد السفلي للخلية A1، يجب أيضًا تغيير الحد العلوي للخلية A2.

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


يحصل على طريقة تحديث الروابط الخارجية عند فتح المصنف.

انظر [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


يحصل على رد النداء للتحذير.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWindowHeight() {#getWindowHeight--}
```
public double getWindowHeight()
```


ارتفاع النافذة، بوحدة النقطة.

**Returns:**
double
### getWindowHeightCM() {#getWindowHeightCM--}
```
public double getWindowHeightCM()
```


ارتفاع النافذة، بوحدة السنتيمتر.

**Returns:**
double
### getWindowHeightInch() {#getWindowHeightInch--}
```
public double getWindowHeightInch()
```


ارتفاع النافذة، بوحدة البوصة.

**Returns:**
double
### getWindowLeft() {#getWindowLeft--}
```
public double getWindowLeft()
```


المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة، بوحدة النقطة.

**Returns:**
double
### getWindowLeftCM() {#getWindowLeftCM--}
```
public double getWindowLeftCM()
```


المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. بوحدة السنتيمتر.

**Returns:**
double
### getWindowLeftInch() {#getWindowLeftInch--}
```
public double getWindowLeftInch()
```


المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. بوحدة البوصة.

**Returns:**
double
### getWindowTop() {#getWindowTop--}
```
public double getWindowTop()
```


المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة النقطة.

**Returns:**
double
### getWindowTopCM() {#getWindowTopCM--}
```
public double getWindowTopCM()
```


المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة السنتيمتر.

**Returns:**
double
### getWindowTopInch() {#getWindowTopInch--}
```
public double getWindowTopInch()
```


المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة البوصة.

**Returns:**
double
### getWindowWidth() {#getWindowWidth--}
```
public double getWindowWidth()
```


عرض النافذة، بوحدة النقطة.

**Returns:**
double
### getWindowWidthCM() {#getWindowWidthCM--}
```
public double getWindowWidthCM()
```


عرض النافذة، بوحدة السنتيمتر.

**Returns:**
double
### getWindowWidthInch() {#getWindowWidthInch--}
```
public double getWindowWidthInch()
```


عرض النافذة، بوحدة البوصة.

**Returns:**
double
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


يشير إلى ما إذا كان يجب أن يكون متوافقًا مع WPS.

**Returns:**
boolean
### getWriteProtection() {#getWriteProtection--}
```
public WriteProtection getWriteProtection()
```


يوفر الوصول إلى خيارات حماية الكتابة في دفتر العمل.

**Returns:**
[WriteProtection](../../com.aspose.cells/writeprotection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDefaultEncrypted() {#isDefaultEncrypted--}
```
public boolean isDefaultEncrypted()
```


يشير إلى ما إذا كان سيتم تشفير دفتر العمل باستخدام كلمة مرور افتراضية إذا تم قفل الهيكل والنوافذ لدفتر العمل.

**Remarks**

القيمة الافتراضية الآن هي false. وهي نفس MS Excel 2013.

**Returns:**
boolean
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


يحصل على قيمة تشير إلى ما إذا كانت كلمة المرور مطلوبة لفتح هذا دفتر العمل.

**Returns:**
boolean
### isHScrollBarVisible() {#isHScrollBarVisible--}
```
public boolean isHScrollBarVisible()
```


يحصل على قيمة تشير إلى ما إذا كان جدول البيانات المُنشأ سيحتوي على شريط تمرير أفقي.

**Remarks**

القيمة الافتراضية هي true.

**Example**

الكود التالي يجعل شريط التمرير الأفقي غير مرئي لجدول البيانات.

```
         // Hide the horizontal scroll bar of the Excel file.
         settings.setHScrollBarVisible(false);
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


يشير إلى ما إذا كان هذا دفتر العمل مخفيًا.

**Returns:**
boolean
### isMinimized() {#isMinimized--}
```
public boolean isMinimized()
```


يمثل ما إذا كان جدول البيانات المُنشأ سيفتح مصغرًا.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


يحصل على قيمة تشير إلى ما إذا كان الهيكل أو نافذة دفتر العمل محميًا.

**Returns:**
boolean
### isVScrollBarVisible() {#isVScrollBarVisible--}
```
public boolean isVScrollBarVisible()
```


يحصل على قيمة تشير إلى ما إذا كان جدول البيانات المُنشأ سيحتوي على شريط تمرير عمودي.

**Remarks**

القيمة الافتراضية هي true.

**Example**

الكود التالي يجعل شريط التمرير العمودي غير مرئي لجدول البيانات.

```
         	// Hide the vertical scroll bar of the Excel file.
         settings.setVScrollBarVisible(false);
```

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


يضبط مؤلف الملف.

**Remarks**

لم يتم تعيينه، تحقق أولاً من [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--)، ثم تحقق من مستخدم البيئة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


يحدد قيمة منطقية تشير إلى أن التطبيق يضغط الصور تلقائيًا في دفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


يشير إلى ما إذا كان الملف محددًا للاستعادة التلقائية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


يحدد الإصدار العام المتدرج للتطبيق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


يشير إلى ما إذا كان يتم فحص التوافق مع الإصدارات السابقة عند حفظ دفتر العمل.

**Remarks**

القيمة الافتراضية هي true. فقط لملفات Excel97-2003 xls أو xlt.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


يشير إلى ما إذا كان يتم فحص تنسيق الأرقام المخصص عند تعيين Style.Custom.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا عبر Cell.PutValue(string)، إذا كانت هذه الخاصية true ستحصل على استثناء. إذا كانت false، سنقبل قيمة السلسلة التي أدخلتها كقيمة للخلية بحيث يمكنك لاحقًا إخراج القيمة الكاملة للملفات الأخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


يحدد إصدار OOXML للمستند الناتج. القيمة الافتراضية هي Ecma376\_2006.

انظر [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

فقط لملفات .xlsx.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


يشير إلى ما إذا كان التطبيق قد حفظ ملف دفتر العمل آخر مرة بعد تعطل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


يشير إلى ما إذا كان التطبيق قد فتح دفتر العمل آخر مرة لاستعادة البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


يضبط قيمة تمثل ما إذا كان دفتر العمل يستخدم نظام التاريخ 1904.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


يشير إلى ما إذا كان سيتم تشفير دفتر العمل باستخدام كلمة مرور افتراضية إذا تم قفل الهيكل والنوافذ لدفتر العمل.

**Remarks**

القيمة الافتراضية الآن هي false. وهي نفس MS Excel 2013.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDefaultImageResolution(int value) {#setDefaultImageResolution-int-}
```
public void setDefaultImageResolution(int value)
```


يضبط الدقة الافتراضية للصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDiscardImageEditData(boolean value) {#setDiscardImageEditData-boolean-}
```
public void setDiscardImageEditData(boolean value)
```


يشير إلى ما إذا كان يتم تجاهل بيانات تحرير الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


يشير إلى ما إذا كان وكيفية عرض الكائنات في دفتر العمل.

انظر [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


تمكين الماكرو؛

**Remarks**

الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في مصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


يضبط علامة تبويب ورقة العمل الأولى المرئية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


يضبط إعدادات العولمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان جدول البيانات المُنشأ سيحتوي على شريط تمرير أفقي.

**Remarks**

القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


يشير إلى ما إذا كان هذا دفتر العمل مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


يضبط ما إذا كان سيتم إخفاء قائمة الحقول لجدول المحور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


يضبط لغة واجهة المستخدم لإصدار المصنف بناءً على CountryCode الذي حفظ الملف.

انظر [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


يضبط اللغة المستخدمة في هذا المصنف.

**Remarks**

يرجع null إذا لم يتم تعيين لا Locale ولا [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Locale |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


يضبط الحد الأقصى لعدد الصفوف للمعادلة المشتركة.

**Remarks**

إذا كان الرقم كبيرًا جدًا، فإن الفلتر التلقائي يعمل ببطء شديد في MS Excel 2013.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMaxUniqueItemsPerField(int value) {#setMaxUniqueItemsPerField-int-}
```
public void setMaxUniqueItemsPerField(int value)
```


يضبط الحد الأقصى للعناصر الفريدة لكل حقل

**Remarks**

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


يضبط خيارات استخدام الذاكرة. سيتم اعتبار الخيار الجديد كخيار افتراضي للأوراق العمل التي تم إنشاؤها حديثًا ولكنه لا يؤثر على الأوراق الموجودة.

انظر [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

لمزيد من التفاصيل حول وضع الذاكرة، يرجى الاطلاع على [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


يمثل ما إذا كان جدول البيانات المُنشأ سيفتح مصغرًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


يضبط الفاصل العشري لتنسيق/تحليل القيم الرقمية. الافتراضي هو الفاصل العشري للمنطقة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


يضبط الحرف الذي يفصل مجموعات الأرقام إلى يسار الفاصل العشري في القيم الرقمية. الافتراضي هو فاصل المجموعات للمنطقة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char |  |

### setPageOrientationType(int pageOrientationType) {#setPageOrientationType-int-}
```
public void setPageOrientationType(int pageOrientationType)
```


اضبط نوع اتجاه الطباعة للمصنف بأكمله.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pageOrientationType | int | [PageOrientationType](../../com.aspose.cells/pageorientationtype). نوع توجيه الصفحة |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


يضبط حجم ورق الطباعة الافتراضي.

انظر [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

إذا لم يكن هناك إعداد لحجم الورق، سيستخدم MS Excel إعداد الطابعة الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


يمثل كلمة مرور تشفير ملف المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPropertiesFollowChartPoint(boolean value) {#setPropertiesFollowChartPoint-boolean-}
```
public void setPropertiesFollowChartPoint(boolean value)
```


يشير إلى ما إذا كانت خصائص نقاط البيانات وملصقات البيانات في جميع المخططات في هذا المصنف تتبع مرجعها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


يشير إلى ما إذا كان ضبط خاصية [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) عند إدخال قيمة النص (التي تبدأ بعلامة اقتباس مفردة) إلى الخلية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


يضبط الإعدادات الإقليمية للمصنف.

انظر [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. الإعدادات الإقليمية التي يستخدمها مكوّن Aspose.Cells لدفتر عمل تم تحميله من ملف قالب: i). بالنسبة لملف XLS، هناك حقول معرفة للإعدادات الإقليمية وتقوم MS Excel بحفظ بيانات الإعدادات الإقليمية في الملف عند حفظ ملف XLS. لذلك، نستخدم المنطقة المحفوظة في ملف القالب للدفتر. إذا لم ترغب في استخدام المنطقة المحفوظة في ملف XLS، يرجى إعادة تعيينها إلى القيمة المتوقعة (مثل CountryCode.Default) بعد تحميل ملف القالب. كما أننا نحفظ القيمة المحددة من قبل المستخدم (باستخدام هذه الطريقة) في الملف أيضًا عند حفظ ملف XLS. ii). بالنسبة لتنسيقات الملفات الأخرى، مثل XLSX، XLSB... إلخ، لا توجد حقل معرف للإعدادات الإقليمية في مواصفات تنسيق الملف. لذلك، نستخدم الإعدادات الإقليمية لبيئة التطبيق للدفتر. ولا يمكن الاحتفاظ بالقيمة المحددة من قبل المستخدم (باستخدام هذه الطريقة) للملفات المولدة بتلك التنسيقات. 2. لتأثير العرض في MS Excel: الإعدادات الإقليمية المطبقة هنا يمكن أن تؤثر فقط أثناء التشغيل مع مكوّن Aspose.Cells وليس عند عرض الملف المولد باستخدام MS Excel. حتى بالنسبة لملف XLS المولد الذي تم حفظ بيانات الإعدادات الإقليمية فيه، عند عرضه/تحريره باستخدام MS Excel، تكون المنطقة المستخدمة لتنسيق القيم بواسطة MS Excel دائمًا هي الإعدادات الإقليمية الافتراضية للبيئة التي يعمل فيها MS Excel، وليس تلك المحفوظة في الملف. هذا سلوك MS Excel ولا يمكن تغييره عبر الشيفرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


صحيح إذا كان يمكن إزالة المعلومات الشخصية من المصنف المحدد.

**Remarks**

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


يشير إلى ما إذا كان التطبيق قد فتح المصنف في وضع الأمان أو الإصلاح آخر مرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


يضبط موفر الدفق للموارد الخارجية، مثل تحميل بيانات الصورة للصور من النوع \"LinkToFile\".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShapeDisplayType(int value) {#setShapeDisplayType-int-}
```
public void setShapeDisplayType(int value)
```


يضبط طريقة عرض التطبيق للأشكال في هذا المصنف

انظر [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان المصنف مشتركًا.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


عرض شريط علامات تبويب ورقة العمل (بـ 1/1000 من عرض النافذة).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


يضبط قيمة ما إذا كانت علامات تبويب المصنف معروضة.

**Remarks**

القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


يضبط عدد الأرقام ذات الدقة. القيمة الافتراضية هي [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

يمكن أن يكون فقط 15 أو 17 الآن. ملاحظة: هذا العضو أصبح مهجورًا الآن. بدلاً من ذلك، يرجى استخدام [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public void setSignificantDigitsType(int value)
```


يضبط نوع الأرقام ذات الدقة لإخراج القيم الرقمية في دفتر العمل هذا. القيمة الافتراضية هي [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

انظر [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


يضبط موفر الدفق للموارد الخارجية.

**Remarks**

ملاحظة: هذا العضو أصبح مهجورًا الآن. بدلاً من ذلك، يرجى استخدام خاصية ResourceProvider. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


يشير إلى ما إذا كان يتم تحديث حدود الخلايا المجاورة.

**Remarks**

القيمة الافتراضية هي false. على سبيل المثال: إذا تم تحديث الحد السفلي للخلية A1، يجب أيضًا تغيير الحد العلوي للخلية A2.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


يضبط طريقة تحديث الروابط الخارجية عند فتح المصنف.

انظر [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان جدول البيانات المُنشأ سيحتوي على شريط تمرير عمودي.

**Remarks**

القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


يضبط رد النداء للتحذير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


ارتفاع النافذة، بوحدة النقطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


ارتفاع النافذة، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


ارتفاع النافذة، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة، بوحدة النقطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة النقطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


عرض النافذة، بوحدة النقطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


عرض النافذة، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


عرض النافذة، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


يشير إلى ما إذا كان يجب أن يكون متوافقًا مع WPS.

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

