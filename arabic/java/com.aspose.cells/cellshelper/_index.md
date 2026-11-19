---
title: "CellsHelper"
second_title: "Aspose.Cells for Java API Reference"
description: "يوفر وظائف مساعدة."
type: docs
url: /ar/java/com.aspose.cells/cellshelper/
---

**Inheritance:**
java.lang.Object
```
public class CellsHelper
```

يوفر وظائف مساعدة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)](#addAddInFunction-java.lang.String-int-int-int---int-) | إضافة وظيفة الإضافة. |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | يحصل على اسم الخلية وفقًا لصفها وعمودها. |
| [cellNameToIndex(String cellName)](#cellNameToIndex-java.lang.String-) | يحصل على صف الخلية وعمودها وفقًا لاسمها. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | يحصل على اسم العمود وفقًا لمؤشر العمود. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | يحصل على مؤشر العمود وفقًا لاسم العمود. |
| [convertA1FormulaToR1C1(String formula, int row, int column)](#convertA1FormulaToR1C1-java.lang.String-int-int-) | يحوّل صيغة A1 للخلية إلى صيغة r1c1. |
| [convertR1C1FormulaToA1(String r1c1Formula, int row, int column)](#convertR1C1FormulaToA1-java.lang.String-int-int-) | يحوّل صيغة r1c1 للخلية إلى صيغة A1. |
| [createSafeSheetName(String nameProposal)](#createSafeSheetName-java.lang.String-) | يتحقق من اسم الورقة المعطى وينشئ اسمًا صالحًا عند الحاجة. |
| [createSafeSheetName(String nameProposal, char replaceChar)](#createSafeSheetName-java.lang.String-char-) | يتحقق من اسم الورقة المعطى وينشئ اسمًا صالحًا عند الحاجة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAltStartPath()](#getAltStartPath--) | يحصل على مسار بدء التشغيل البديل، الذي يُشار إليه في بعض مراجع الصيغ الخارجية. |
| [getCacheFolder()](#getCacheFolder--) | يحصل على المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [getClass()](#getClass--) |  |
| [getCustomImplementationFactory()](#getCustomImplementationFactory--) | يحصل على المصنع لإنشاء مثيلات بتنفيذ خاص. |
| [getDPI()](#getDPI--) | يحصل على DPI للجهاز. |
| [getDateTimeFromDouble(double doubleValue, boolean date1904)](#getDateTimeFromDouble-double-boolean-) | حوّل القيمة المزدوجة إلى قيمة تاريخ ووقت. |
| [getDoubleFromDateTime(DateTime dateTime, boolean date1904)](#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-) | حوّل التاريخ والوقت إلى قيمة مزدوجة. |
| [getLibraryPath()](#getLibraryPath--) | يحصل على مسار المكتبة الذي يُشار إليه في بعض مراجع الصيغ الخارجية. |
| [getSignificantDigits()](#getSignificantDigits--) | يحصل على عدد الأرقام ذات الدقة. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | يحصل على النوع الافتراضي للأرقام ذات الدقة لإخراج القيم الرقمية. |
| [getStartupPath()](#getStartupPath--) | يحصل على مسار بدء التشغيل، الذي يُشار إليه في بعض مراجع الصيغ الخارجية. |
| [getTextWidth(String text, Font font, double scaling)](#getTextWidth-java.lang.String-com.aspose.cells.Font-double-) | احصل على عرض النص بوحدة النقاط. |
| [getUsedColors(Workbook workbook)](#getUsedColors-com.aspose.cells.Workbook-) | يحصل على جميع الألوان المستخدمة في المصنف. |
| [getVersion()](#getVersion--) | احصل على نسخة الإصدار. |
| [hashCode()](#hashCode--) |  |
| [isCloudPlatform()](#isCloudPlatform--) | يرجى تعيين هذه الخاصية إلى True عند التشغيل على منصة سحابية، مثل: Azure، AWSLambda، إلخ، |
| [mergeFiles(String[] files, String cachedFile, String destFile)](#mergeFiles-java.lang.String---java.lang.String-java.lang.String-) | يدمج بعض ملفات xls الكبيرة إلى ملف xls واحد. |
| [needQuoteInFormula(String sheetName)](#needQuoteInFormula-java.lang.String-) | يشير إلى ما إذا كان يجب أن يكون اسم الورقة محاطًا بعلامات اقتباس مفردة |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rowIndexToName(int row)](#rowIndexToName-int-) | يحصل على اسم الصف وفقًا لمؤشر الصف. |
| [rowNameToIndex(String rowName)](#rowNameToIndex-java.lang.String-) | يحصل على مؤشر الصف وفقًا لاسم الصف. |
| [setAltStartPath(String value)](#setAltStartPath-java.lang.String-) | يضبط مسار بدء التشغيل البديل، الذي يُشار إليه في بعض مراجع الصيغ الخارجية. |
| [setCacheFolder(String cache)](#setCacheFolder-java.lang.String-) | يضبط المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [setCloudPlatform(boolean value)](#setCloudPlatform-boolean-) | يرجى تعيين هذه الخاصية إلى True عند التشغيل على منصة سحابية، مثل: Azure، AWSLambda، إلخ، |
| [setCustomImplementationFactory(CustomImplementationFactory value)](#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-) | يضبط المصنع لإنشاء كائنات بتنفيذ خاص. |
| [setDPI(double value)](#setDPI-double-) | يحصل على DPI للجهاز. |
| [setLibraryPath(String value)](#setLibraryPath-java.lang.String-) | يضبط مسار المكتبة الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | يضبط عدد الأرقام ذات الدقة. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | يضبط النوع الافتراضي للأرقام ذات الدقة عند إخراج القيم الرقمية. |
| [setStartupPath(String value)](#setStartupPath-java.lang.String-) | يضبط مسار بدء التشغيل الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType) {#addAddInFunction-java.lang.String-int-int-int---int-}
```
public static void addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)
```


إضافة وظيفة الإضافة.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طرق WorksheetCollection.RegisterAddInFunction(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يناير 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دالة | java.lang.String | اسم الدالة. |
| minCountOfParameters | int | الحد الأدنى لعدد المعلمات التي تتطلبها هذه الدالة |
| maxCountOfParameters | int | الحد الأقصى لعدد المعلمات التي تسمح بها هذه الدالة. |
| paramersType | int[] | [ParameterType](../../com.aspose.cells/parametertype). نوع المعلمات المتوقعة للدالة |
| functionValueType | int | [ParameterType](../../com.aspose.cells/parametertype). نوع قيمة الدالة. |

### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


يحصل على اسم الخلية وفقًا لصفها وعمودها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| عمود | int | فهرس العمود. |

**Returns:**
java.lang.String - اسم الخلية.
### cellNameToIndex(String cellName) {#cellNameToIndex-java.lang.String-}
```
public static int[] cellNameToIndex(String cellName)
```


يحصل على صف الخلية وعمودها وفقًا لاسمها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية |

**Returns:**
int[] - [0] هو فهرس الصف و[1] هو فهرس العمود.
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


يحصل على اسم العمود وفقًا لمؤشر العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |

**Returns:**
java.lang.String - اسم العمود.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


يحصل على مؤشر العمود وفقًا لاسم العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnName | java.lang.String | اسم العمود. |

**Returns:**
int - فهرس العمود.
### convertA1FormulaToR1C1(String formula, int row, int column) {#convertA1FormulaToR1C1-java.lang.String-int-int-}
```
public static String convertA1FormulaToR1C1(String formula, int row, int column)
```


يحوّل صيغة A1 للخلية إلى صيغة r1c1.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طريقة Worksheet.ConvertFormulaReferenceStyle(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة A1. |
| صف | int | فهرس الصف للخلية. |
| عمود | int | فهرس العمود للخلية. |

**Returns:**
java.lang.String - صيغة R1C1.
### convertR1C1FormulaToA1(String r1c1Formula, int row, int column) {#convertR1C1FormulaToA1-java.lang.String-int-int-}
```
public static String convertR1C1FormulaToA1(String r1c1Formula, int row, int column)
```


يحوّل صيغة r1c1 للخلية إلى صيغة A1.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طريقة Worksheet.ConvertFormulaReferenceStyle(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| r1c1Formula | java.lang.String | صيغة r1c1. |
| صف | int | فهرس الصف للخلية. |
| عمود | int | فهرس العمود للخلية. |

**Returns:**
java.lang.String - صيغة A1.
### createSafeSheetName(String nameProposal) {#createSafeSheetName-java.lang.String-}
```
public static String createSafeSheetName(String nameProposal)
```


يتحقق من اسم الورقة المُعطى وينشئ اسمًا صالحًا عند الحاجة. إذا كان اسم الورقة المُعطى يتوافق مع قواعد أسماء أوراق Excel، يتم إرجاعه. وإلا سيتم قطع السلسلة إذا تجاوز الطول الحد المسموح وسيتم استبدال الأحرف غير الصالحة بـ ' ', ثم إرجاع قيمة السلسلة المعاد بناؤها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| nameProposal | java.lang.String | اسم الورقة المراد استخدامه |

**Returns:**
java.lang.String -
### createSafeSheetName(String nameProposal, char replaceChar) {#createSafeSheetName-java.lang.String-char-}
```
public static String createSafeSheetName(String nameProposal, char replaceChar)
```


يتحقق من اسم الورقة المُعطى وينشئ اسمًا صالحًا عند الحاجة. إذا كان اسم الورقة المُعطى يتوافق مع قواعد أسماء أوراق Excel، يتم إرجاعه. وإلا سيتم قطع السلسلة إذا تجاوز الطول الحد المسموح وسيتم استبدال الأحرف غير الصالحة بالحرف المُعطى، ثم إرجاع قيمة السلسلة المعاد بناؤها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| nameProposal | java.lang.String | اسم الورقة المراد استخدامه |
| replaceChar | char | الحرف الذي سيُستخدم لاستبدال الأحرف غير الصالحة في اسم الورقة المُعطى |

**Returns:**
java.lang.String -
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
### getAltStartPath() {#getAltStartPath--}
```
public static String getAltStartPath()
```


يحصل على مسار بدء التشغيل البديل، الذي يُشار إليه في بعض مراجع الصيغ الخارجية.

**Returns:**
java.lang.String
### getCacheFolder() {#getCacheFolder--}
```
public static String getCacheFolder()
```


يحصل على المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

**Remarks**

تُستخدم ملفات التخزين المؤقت عادةً لبعض الميزات لتحسين أداء الذاكرة، مثل حفظ مجموعة بيانات كبيرة إلى ملف xls، أو استخدام وضع الذاكرة مع التخزين المؤقت للملفات لنموذج الخلايا.

**Returns:**
java.lang.String - المجلد لملفات التخزين المؤقت الذي تم تحديده. إذا لم يتم تحديده، سيتم إرجاع null وسيتم استخدام المسار المؤقت للنظام عند الحاجة.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomImplementationFactory() {#getCustomImplementationFactory--}
```
public static CustomImplementationFactory getCustomImplementationFactory()
```


يحصل على المصنع لإنشاء مثيلات بتنفيذ خاص.

**Returns:**
[CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory)
### getDPI() {#getDPI--}
```
public static double getDPI()
```


يحصل على DPI للجهاز.

**Remarks**

**Returns:**
double
### getDateTimeFromDouble(double doubleValue, boolean date1904) {#getDateTimeFromDouble-double-boolean-}
```
public static DateTime getDateTimeFromDouble(double doubleValue, boolean date1904)
```


حوّل القيمة المزدوجة إلى قيمة تاريخ ووقت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| doubleValue | double | القيمة المزدوجة. |
| date1904 | boolean | نظام تاريخ 1904. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - 
### getDoubleFromDateTime(DateTime dateTime, boolean date1904) {#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-}
```
public static double getDoubleFromDateTime(DateTime dateTime, boolean date1904)
```


حوّل التاريخ والوقت إلى قيمة مزدوجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | التاريخ والوقت. |
| date1904 | boolean | نظام تاريخ 1904. |

**Returns:**
double -
### getLibraryPath() {#getLibraryPath--}
```
public static String getLibraryPath()
```


يحصل على مسار المكتبة الذي يُشار إليه في بعض مراجع الصيغ الخارجية.

**Returns:**
java.lang.String
### getSignificantDigits() {#getSignificantDigits--}
```
public static int getSignificantDigits()
```


يحصل على عدد الأرقام المهمة. القيمة الافتراضية هي 17.

**Remarks**

يمكن أن يكون فقط 15 أو 17 الآن. ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public static int getSignificantDigitsType()
```


يحصل على النوع الافتراضي للأرقام المهمة عند إخراج القيم الرقمية. القيمة الافتراضية هي [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

انظر [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getStartupPath() {#getStartupPath--}
```
public static String getStartupPath()
```


يحصل على مسار بدء التشغيل، الذي يُشار إليه في بعض مراجع الصيغ الخارجية.

**Returns:**
java.lang.String
### getTextWidth(String text, Font font, double scaling) {#getTextWidth-java.lang.String-com.aspose.cells.Font-double-}
```
public static double getTextWidth(String text, Font font, double scaling)
```


احصل على عرض النص بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | النص. |
| font | [Font](../../com.aspose.cells/font) | خط النص. |
| تحجيم | double | تحجيم النص. |

**Returns:**
double -
### getUsedColors(Workbook workbook) {#getUsedColors-com.aspose.cells.Workbook-}
```
public static Color[] getUsedColors(Workbook workbook)
```


يحصل على جميع الألوان المستخدمة في المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | كائن دفتر العمل. |

**Returns:**
com.aspose.cells.Color[] - الألوان المستخدمة.
### getVersion() {#getVersion--}
```
public static String getVersion()
```


احصل على نسخة الإصدار.

**Returns:**
java.lang.String - نسخة الإصدار.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCloudPlatform() {#isCloudPlatform--}
```
public static boolean isCloudPlatform()
```


يرجى تعيين هذه الخاصية إلى True عند التشغيل على منصة سحابية، مثل: Azure، AWSLambda، إلخ،

**Returns:**
boolean
### mergeFiles(String[] files, String cachedFile, String destFile) {#mergeFiles-java.lang.String---java.lang.String-java.lang.String-}
```
public static void mergeFiles(String[] files, String cachedFile, String destFile)
```


يدمج بعض ملفات xls الكبيرة إلى ملف xls واحد.

**Remarks**

هذه الطريقة تدعم فقط دمج البيانات والأنماط والصيغ إلى الملف الجديد. يُستخدم الملف المؤقت لتخزين بعض البيانات المؤقتة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ملفات | java.lang.String[] | الملفات. |
| cachedFile | java.lang.String | الملف المؤقت. |
| destFile | java.lang.String | ملف الوجهة. |

### needQuoteInFormula(String sheetName) {#needQuoteInFormula-java.lang.String-}
```
public static boolean needQuoteInFormula(String sheetName)
```


يشير إلى ما إذا كان يجب أن يكون اسم الورقة محاطًا بعلامات اقتباس مفردة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String | اسم الورقة |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rowIndexToName(int row) {#rowIndexToName-int-}
```
public static String rowIndexToName(int row)
```


يحصل على اسم الصف وفقًا لمؤشر الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |

**Returns:**
java.lang.String - اسم الصف.
### rowNameToIndex(String rowName) {#rowNameToIndex-java.lang.String-}
```
public static int rowNameToIndex(String rowName)
```


يحصل على مؤشر الصف وفقًا لاسم الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowName | java.lang.String | اسم الصف. |

**Returns:**
int - فهرس الصف.
### setAltStartPath(String value) {#setAltStartPath-java.lang.String-}
```
public static void setAltStartPath(String value)
```


يضبط مسار بدء التشغيل البديل، الذي يُشار إليه في بعض مراجع الصيغ الخارجية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCacheFolder(String cache) {#setCacheFolder-java.lang.String-}
```
public static void setCacheFolder(String cache)
```


يضبط المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

**Remarks**

تُستخدم ملفات التخزين المؤقت عادةً لبعض الميزات لتحسين أداء الذاكرة، مثل حفظ مجموعة بيانات كبيرة إلى ملف xls، أو استخدام وضع الذاكرة مع التخزين المؤقت للملفات لنموذج الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مخزن مؤقت | java.lang.String | مجلد للملفات المؤقتة التي قد تُستخدم كمخزن بيانات. |

### setCloudPlatform(boolean value) {#setCloudPlatform-boolean-}
```
public static void setCloudPlatform(boolean value)
```


يرجى تعيين هذه الخاصية إلى True عند التشغيل على منصة سحابية، مثل: Azure، AWSLambda، إلخ،

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCustomImplementationFactory(CustomImplementationFactory value) {#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-}
```
public static void setCustomImplementationFactory(CustomImplementationFactory value)
```


يضبط المصنع لإنشاء كائنات بتنفيذ خاص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory) |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


يحصل على DPI للجهاز.

**Remarks**

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLibraryPath(String value) {#setLibraryPath-java.lang.String-}
```
public static void setLibraryPath(String value)
```


يضبط مسار المكتبة الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public static void setSignificantDigits(int value)
```


يضبط عدد الأرقام ذات الدقة. القيمة الافتراضية هي 17.

**Remarks**

يمكن أن يكون فقط 15 أو 17 الآن. ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public static void setSignificantDigitsType(int value)
```


يضبط النوع الافتراضي للأرقام ذات الدقة عند إخراج القيم الرقمية. القيمة الافتراضية هي [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

انظر [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStartupPath(String value) {#setStartupPath-java.lang.String-}
```
public static void setStartupPath(String value)
```


يضبط مسار بدء التشغيل الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

