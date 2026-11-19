---
title: "Workbook"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل كائن الجذر لإنشاء جدول بيانات Excel."
type: docs
url: /ar/java/com.aspose.cells/workbook/
---

**Inheritance:**
java.lang.Object
```
public class Workbook
```

يمثل كائن الجذر لإنشاء جدول بيانات Excel.

**Remarks**

فئة Workbook تشير إلى جدول بيانات Excel. يمكن لكل جدول بيانات أن يحتوي على عدة أوراق عمل. الميزة الأساسية للفئة هي فتح وحفظ ملفات Excel الأصلية. تحتوي الفئة على بعض الميزات المتقدمة مثل نسخ البيانات من Workbooks أخرى، دمج Workbooks اثنتين، تحويل Excel إلى PDF، تحويل Excel إلى صورة وحماية جدول بيانات Excel.

**Example**

المثال التالي يقوم بتحميل Workbook من ملف Excel اسمه designer.xls ويجعل أشرطة التمرير الأفقية والعمودية غير مرئية. ثم يستبدل قيمتين نصيتين بقيمة عددية صحيحة وقيمة نصية على التوالي داخل جدول البيانات وأخيرًا يحفظ المصنف كملف Excel xlsx.

```
         //Open a designer file
         String designerFile = "designer.xls";
         Workbook workbook = new Workbook(designerFile);
 
         //Set scroll bars
         workbook.getSettings().setHScrollBarVisible(false);
         workbook.getSettings().setVScrollBarVisible(false);
 
         //Replace the placeholder string with new values
         int newInt = 100;
         workbook.replace("OldInt", newInt);
 
         String newString = "Hello!";
         workbook.replace("OldString", newString);
         workbook.save("result.xlsx");
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Workbook()](#Workbook--) | ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(int fileFormatType)](#Workbook-int-) | ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(LoadOptions loadOptions)](#Workbook-com.aspose.cells.LoadOptions-) | ينشئ مثيلًا جديدًا فارغًا من الفئة [Workbook](../../com.aspose.cells/workbook) مع الخيارات |
| [Workbook(String file)](#Workbook-java.lang.String-) | ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook) ويفتح ملفًا. |
| [Workbook(InputStream stream)](#Workbook-java.io.InputStream-) | ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook) ويفتح تدفقًا. |
| [Workbook(String file, LoadOptions loadOptions)](#Workbook-java.lang.String-com.aspose.cells.LoadOptions-) | ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook) ويفتح ملفًا. |
| [Workbook(InputStream stream, LoadOptions loadOptions)](#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-) | ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook) ويفتح تدفقًا. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [acceptAllRevisions()](#acceptAllRevisions--) | يقبل جميع التغييرات المتتبعة في دفتر العمل. |
| [addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | يضيف توقيعًا رقميًا إلى ملف جدول بيانات OOXML (Excel2007 وما بعده). |
| [calculateFormula()](#calculateFormula--) | يحسب نتيجة الصيغ. |
| [calculateFormula(boolean ignoreError)](#calculateFormula-boolean-) | يحسب نتيجة الصيغ. |
| [calculateFormula(CalculationOptions options)](#calculateFormula-com.aspose.cells.CalculationOptions-) | حساب الصيغ في هذا دفتر العمل. |
| [changePalette(Color color, int index)](#changePalette-com.aspose.cells.Color-int-) | يغيّر لوحة الألوان لجدول البيانات في الفهرس المحدد. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | يغلق الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات. |
| [combine(Workbook secondWorkbook)](#combine-com.aspose.cells.Workbook-) | يجمع كائن دفتر عمل آخر. |
| [copy(Workbook source)](#copy-com.aspose.cells.Workbook-) | ينسخ البيانات من كائن دفتر عمل المصدر. |
| [copy(Workbook source, CopyOptions copyOptions)](#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-) | ينسخ كائن دفتر عمل آخر. |
| [copyTheme(Workbook source)](#copyTheme-com.aspose.cells.Workbook-) | ينسخ السمة من دفتر عمل آخر. |
| [createBuiltinStyle(int type)](#createBuiltinStyle-int-) | ينشئ نمطًا مدمجًا حسب النوع المحدد. |
| [createCellsColor()](#createCellsColor--) | ينشئ كائنًا من نوع [CellsColor](../../com.aspose.cells/cellscolor). |
| [createStyle()](#createStyle--) | ينشئ نمطًا جديدًا. |
| [createStyle(boolean cloneDefaultStyle)](#createStyle-boolean-) | ينشئ نمطًا جديدًا. |
| [customTheme(String themeName, Color[] colors)](#customTheme-java.lang.String-com.aspose.cells.Color---) | يخصص السمة. |
| [dispose()](#dispose--) | ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportXml(String mapName, OutputStream stream)](#exportXml-java.lang.String-java.io.OutputStream-) | يصدّر بيانات XML المرتبطة بخريطة XML المحددة. |
| [exportXml(String mapName, String path)](#exportXml-java.lang.String-java.lang.String-) | يصدّر بيانات XML المرتبطة بخريطة XML المحددة. |
| [getAbsolutePath()](#getAbsolutePath--) | يحصل على المسار المطلق للملف. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | يرجع مجموعة [DocumentProperty](../../com.aspose.cells/documentproperty) تمثل جميع خصائص المستند المدمجة في جدول البيانات. |
| [getCellsDataTableFactory()](#getCellsDataTableFactory--) | يحصل على المصنع لبناء ICellsDataTable من كائنات مخصصة |
| [getClass()](#getClass--) |  |
| [getColors()](#getColors--) | يعيد الألوان في لوحة الألوان لجدول البيانات. |
| [getContentTypeProperties()](#getContentTypeProperties--) | يحصل على قائمة كائنات [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) في دفتر العمل. |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--) | يحصل على عدد الأنماط في مجموعة الأنماط. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | يرجع مجموعة [DocumentProperty](../../com.aspose.cells/documentproperty) تمثل جميع خصائص المستند المخصصة في جدول البيانات. |
| [getCustomXmlParts()](#getCustomXmlParts--) | يمثل Custom XML Data Storage Part (بيانات XML مخصصة داخل حزمة). |
| [getDataConnections()](#getDataConnections--) | يحصل على مجموعة [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getDataMashup()](#getDataMashup--) | يحصل على بيانات الدمج. |
| [getDataModel()](#getDataModel--) | يحصل على نموذج البيانات في دفتر العمل. |
| [getDataSorter()](#getDataSorter--) | يحصل على كائن DataSorter لفرز البيانات. |
| [getDefaultStyle()](#getDefaultStyle--) | يحصل على كائن [Style](../../com.aspose.cells/style) الافتراضي لدفتر العمل. |
| [getDigitalSignature()](#getDigitalSignature--) | يحصل على التوقيع الرقمي من الملف. |
| [getFileFormat()](#getFileFormat--) | يحصل على تنسيق الملف. |
| [getFileName()](#getFileName--) | يحصل على اسم الملف الحالي. |
| [getFonts()](#getFonts--) | يحصل على جميع الخطوط في مجموعة الأنماط. |
| [getInterruptMonitor()](#getInterruptMonitor--) | يحصل على مراقب المقاطعة. |
| [getMatchingColor(Color rawColor)](#getMatchingColor-com.aspose.cells.Color-) | ابحث عن اللون الأنسب في لوحة الألوان الحالية. |
| [getNamedStyle(String name)](#getNamedStyle-java.lang.String-) | يحصل على النمط المسمى في مجموعة الأنماط. |
| [getRibbonXml()](#getRibbonXml--) | يحصل على ملف XML الذي يحدد واجهة الشريط. |
| [getSettings()](#getSettings--) | يمثل إعدادات المصنف. |
| [getStyleInPool(int index)](#getStyleInPool-int-) | يحصل على النمط في مجموعة الأنماط. |
| [getTheme()](#getTheme--) | يحصل على اسم السمة. |
| [getThemeColor(int type)](#getThemeColor-int-) | يحصل على لون السمة. |
| [getVbaProject()](#getVbaProject--) | يحصل على [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) في جدول بيانات. |
| [getWorksheets()](#getWorksheets--) | يحصل على مجموعة [WorksheetCollection](../../com.aspose.cells/worksheetcollection) في جدول البيانات. |
| [hasCustomFunction()](#hasCustomFunction--) | يكشف ما إذا كان هناك دالة مخصصة مستخدمة في هذا المصنف، مثل في صيغة الخلية، أو في الأسماء المعرفة... |
| [hasExernalLinks()](#hasExernalLinks--) | يشير إلى ما إذا كان هذا المصنف يحتوي على روابط خارجية لمصادر بيانات أخرى. |
| [hasMacro()](#hasMacro--) | يشير إلى ما إذا كان هذا جدول البيانات يحتوي على ماكرو/VBA. |
| [hasRevisions()](#hasRevisions--) | يحصل على ما إذا كان المصنف يحتوي على أي تغييرات متتبعة |
| [hashCode()](#hashCode--) |  |
| [importXml(InputStream stream, String sheetName, int row, int col)](#importXml-java.io.InputStream-java.lang.String-int-int-) | يستورد/يحدّث ملف بيانات XML إلى المصنف. |
| [importXml(String url, String sheetName, int row, int col)](#importXml-java.lang.String-java.lang.String-int-int-) | يستورد/يحدّث ملف بيانات XML إلى المصنف. |
| [isColorInPalette(Color color)](#isColorInPalette-com.aspose.cells.Color-) | يتحقق مما إذا كان اللون موجودًا في لوحة ألوان جدول البيانات. |
| [isDigitallySigned()](#isDigitallySigned--) | يشير إلى ما إذا كان هذا جدول البيانات موقعًا رقمياً. |
| [isLicensed()](#isLicensed--) | يشير إلى ما إذا تم تعيين الترخيص. |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--) | يشير إلى ما إذا كان الهيكل أو النافذة محميين بكلمة مرور. |
| [mergeNamedStyles(Workbook source)](#mergeNamedStyles-com.aspose.cells.Workbook-) | يدمج الأنماط المسمية من ملف Excel الآخر. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFormulas(boolean ignoreError)](#parseFormulas-boolean-) | يفكّ تحليل جميع الصيغ التي لم يتم تحليلها عندما تم تحميلها من ملف القالب أو تعيينها إلى خلية. |
| [protect(int protectionType, String password)](#protect-int-java.lang.String-) | يحمي مصنفًا. |
| [protectSharedWorkbook(String password)](#protectSharedWorkbook-java.lang.String-) | يحمي مصنفًا مشتركًا. |
| [refreshAll()](#refreshAll--) | تحديث الأشكال المرتبطة، وجميع جداول المحور والرسوم البيانية بمصدر المحور. |
| [refreshDynamicArrayFormulas(boolean calculate)](#refreshDynamicArrayFormulas-boolean-) | يقوم بتحديث صيغ المصفوفة الديناميكية (تنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية) لن يتم حساب الصيغ الأخرى في المصنف بشكل متكرر حتى إذا تم استخدامها بواسطة صيغ المصفوفة الديناميكية. |
| [refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)](#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-) | يقوم بتحديث صيغ المصفوفة الديناميكية (تنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية) |
| [removeDigitalSignature()](#removeDigitalSignature--) | إزالة التوقيع الرقمي من هذه الورقة. |
| [removeExternalLinks()](#removeExternalLinks--) | إزالة جميع الروابط الخارجية في المصنف. |
| [removeMacro()](#removeMacro--) | إزالة VBA/ماكرو من هذه الورقة. |
| [removePersonalInformation()](#removePersonalInformation--) | إزالة المعلومات الشخصية. |
| [removeUnusedStyles()](#removeUnusedStyles--) | إزالة جميع الأنماط غير المستخدمة. |
| [replace(boolean boolValue, Object newValue)](#replace-boolean-java.lang.Object-) | استبدال قيم الخلايا ببيانات جديدة. |
| [replace(int intValue, Object newValue)](#replace-int-java.lang.Object-) | استبدال قيم الخلايا ببيانات جديدة. |
| [replace(String placeHolder, double newValue)](#replace-java.lang.String-double-) | استبدال قيمة خلية واحدة بعدد مزدوج جديد. |
| [replace(String placeHolder, double[] newValues, boolean isVertical)](#replace-java.lang.String-double---boolean-) | استبدال قيم الخلايا بمصفوفة مزدوجة. |
| [replace(String placeHolder, int newValue)](#replace-java.lang.String-int-) | استبدال قيمة خلية واحدة بعدد صحيح جديد. |
| [replace(String placeHolder, int[] newValues, boolean isVertical)](#replace-java.lang.String-int---boolean-) | استبدال قيم الخلايا بمصفوفة أعداد صحيحة. |
| [replace(String placeHolder, String newValue)](#replace-java.lang.String-java.lang.String-) | استبدال قيمة خلية واحدة بسلسلة نصية جديدة. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | استبدال قيمة خلية واحدة بسلسلة نصية جديدة. |
| [replace(String placeHolder, String[] newValues, boolean isVertical)](#replace-java.lang.String-java.lang.String---boolean-) | استبدال قيمة خلية واحدة بمصفوفة سلاسل نصية جديدة. |
| [save(OutputStream stream, SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.cells.SaveOptions-) | حفظ المصنف إلى الدفق. |
| [save(OutputStream stream, int saveFormat)](#save-java.io.OutputStream-int-) | حفظ المصنف إلى الدفق. |
| [save(String fileName)](#save-java.lang.String-) | حفظ المصنف إلى القرص. |
| [save(String fileName, SaveOptions saveOptions)](#save-java.lang.String-com.aspose.cells.SaveOptions-) | يحفظ المصنف إلى القرص. |
| [save(String fileName, int saveFormat)](#save-java.lang.String-int-) | يحفظ المصنف إلى القرص. |
| [setAbsolutePath(String value)](#setAbsolutePath-java.lang.String-) | تعيين المسار المطلق للملف. |
| [setDefaultStyle(Style value)](#setDefaultStyle-com.aspose.cells.Style-) | تعيين كائن [Style](../../com.aspose.cells/style) الافتراضي للمصنف. |
| [setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | تعيين توقيع رقمي لملف ورقة عمل (Excel2007 وما بعده). |
| [setEncryptionOptions(int encryptionType, int keyLength)](#setEncryptionOptions-int-int-) | تعيين خيارات التشفير. |
| [setFileFormat(int value)](#setFileFormat-int-) | تعيين تنسيق الملف. |
| [setFileName(String value)](#setFileName-java.lang.String-) | تعيين اسم الملف الحالي. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | يضبط مراقب المقاطعة. |
| [setRibbonXml(String value)](#setRibbonXml-java.lang.String-) | تعيين ملف XML الذي يحدد واجهة شريط الأدوات. |
| [setThemeColor(int type, Color color)](#setThemeColor-int-com.aspose.cells.Color-) | يضبط لون السمة |
| [startAccessCache(int opts)](#startAccessCache-int-) | يبدأ الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات. |
| [toString()](#toString--) |  |
| [unprotect(String password)](#unprotect-java.lang.String-) | يفك حماية مصنف. |
| [unprotectSharedWorkbook(String password)](#unprotectSharedWorkbook-java.lang.String-) | يفك حماية مصنف مشترك. |
| [updateCustomFunctionDefinition(CustomFunctionDefinition definition)](#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | يحدّث تعريف الدوال المخصصة. |
| [updateLinkedDataSource(Workbook[] externalWorkbooks)](#updateLinkedDataSource-com.aspose.cells.Workbook---) | إذا كان هذا المصنف يحتوي على روابط خارجية إلى مصدر بيانات آخر، سيحاول Aspose.Cells استرجاع أحدث البيانات من المصادر المعطاة. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Workbook() {#Workbook--}
```
public Workbook()
```


ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook).

**Remarks**

نوع تنسيق الملف الافتراضي هو Xlsx. إذا كنت تريد إنشاء أنواع أخرى من الملفات، يرجى استخدام Workbook(FileFormatType).

**Example**

يعرض الشيفرة التالية كيفية استخدام مُنشئ Workbook لإنشاء وتهيئة نسخة جديدة من الفئة.

```
         Workbook workbook = new Workbook();
```

### Workbook(int fileFormatType) {#Workbook-int-}
```
public Workbook(int fileFormatType)
```


ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook).

**Remarks**

نوع تنسيق الملف الافتراضي هو Excel97To2003.

**Example**

يعرض الشيفرة التالية كيفية استخدام مُنشئ Workbook لإنشاء وتهيئة نسخة جديدة من الفئة بأنواع مختلفة من تنسيقات الملفات.

```
         Workbook workbook = new Workbook(FileFormatType.XLSX);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileFormatType | int | [FileFormatType](../../com.aspose.cells/fileformattype). تنسيق الملف الجديد. |

### Workbook(LoadOptions loadOptions) {#Workbook-com.aspose.cells.LoadOptions-}
```
public Workbook(LoadOptions loadOptions)
```


ينشئ مثيلًا جديدًا فارغًا من الفئة [Workbook](../../com.aspose.cells/workbook) مع الخيارات

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | الخيارات. |

### Workbook(String file) {#Workbook-java.lang.String-}
```
public Workbook(String file)
```


ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook) ويفتح ملفًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ملف | java.lang.String | اسم الملف. |

### Workbook(InputStream stream) {#Workbook-java.io.InputStream-}
```
public Workbook(InputStream stream)
```


ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook) ويفتح تدفقًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | التدفق. |

### Workbook(String file, LoadOptions loadOptions) {#Workbook-java.lang.String-com.aspose.cells.LoadOptions-}
```
public Workbook(String file, LoadOptions loadOptions)
```


ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook) ويفتح ملفًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ملف | java.lang.String | اسم الملف. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | خيارات التحميل |

### Workbook(InputStream stream, LoadOptions loadOptions) {#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-}
```
public Workbook(InputStream stream, LoadOptions loadOptions)
```


ينشئ مثيلًا جديدًا من الفئة [Workbook](../../com.aspose.cells/workbook) ويفتح تدفقًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | التدفق. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | خيارات التحميل |

### acceptAllRevisions() {#acceptAllRevisions--}
```
public void acceptAllRevisions()
```


يقبل جميع التغييرات المتتبعة في دفتر العمل.

### addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


يضيف توقيعًا رقميًا إلى ملف جدول بيانات OOXML (Excel2007 وما بعده).

**Remarks**

يدعم فقط إضافة توقيع رقمي Xmldsig إلى ملف جدول بيانات OOXML

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


يحسب نتيجة الصيغ.

**Remarks**

لجميع الصيغ المدعومة، يرجى الاطلاع على القائمة في https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### calculateFormula(boolean ignoreError) {#calculateFormula-boolean-}
```
public void calculateFormula(boolean ignoreError)
```


يحسب نتيجة الصيغ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ignoreError | boolean | يشير إلى إخفاء الخطأ عند حساب الصيغ. قد يكون الخطأ نتيجة دالة غير مدعومة أو روابط خارجية، إلخ. |

### calculateFormula(CalculationOptions options) {#calculateFormula-com.aspose.cells.CalculationOptions-}
```
public void calculateFormula(CalculationOptions options)
```


حساب الصيغ في هذا دفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | خيارات الحساب |

### changePalette(Color color, int index) {#changePalette-com.aspose.cells.Color-int-}
```
public void changePalette(Color color, int index)
```


يغيّر لوحة الألوان لجدول البيانات في الفهرس المحدد.

**Remarks**

تحتوي اللوحة على 56 مدخلاً، كل منها ممثل بقيمة RGB.

إذا قمت بتعيين لون غير موجود في اللوحة، فلن يتم تطبيقه.

لذلك إذا كنت تريد تعيين لون مخصص، يرجى تعديل اللوحة أولاً.

اللوحة اللونية القياسية هي التالية.

| Color | أحمر | أخضر | أزرق |
| ------- | --- | ----- | ---- |
| أسود | 0 | 0 | 0 |
| أبيض | 255 | 255 | 255 |
| أحمر | 255 | 0 | 0 |
| ليموني | 0 | 255 | 0 |
| أزرق | 0 | 0 | 255 |
| أصفر | 255 | 255 | 0 |
| ماجنتا | 255 | 0 | 255 |
| سماوي | 0 | 255 | 255 |
| مارون | 128 | 0 | 0 |
| أخضر | 0 | 128 | 0 |
| بحري | 0 | 0 | 128 |
| زيتي | 128 | 128 | 0 |
| أرجواني | 128 | 0 | 128 |
| تركوازي | 0 | 128 | 128 |
| فضي | 192 | 192 | 192 |
| رمادي | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Color19 | 255 | 255 | 204 |
| Color20 | 204 | 255 | 255 |
| Color21 | 102 | 0 | 102 |
| لون22 | 255 | 128 | 128 |
| لون23 | 0 | 102 | 204 |
| لون24 | 204 | 204 | 255 |
| لون25 | 0 | 0 | 128 |
| لون26 | 255 | 0 | 255 |
| لون27 | 255 | 255 | 0 |
| لون28 | 0 | 255 | 255 |
| لون29 | 128 | 0 | 128 |
| لون30 | 128 | 0 | 0 |
| لون31 | 0 | 128 | 128 |
| لون32 | 0 | 0 | 255 |
| لون33 | 0 | 204 | 255 |
| لون34 | 204 | 255 | 255 |
| لون35 | 204 | 255 | 204 |
| لون36 | 255 | 255 | 153 |
| لون37 | 153 | 204 | 255 |
| لون38 | 255 | 153 | 204 |
| لون39 | 204 | 153 | 255 |
| لون40 | 255 | 204 | 153 |
| لون41 | 51 | 102 | 255 |
| لون42 | 51 | 204 | 204 |
| لون43 | 153 | 204 | 0 |
| لون44 | 255 | 204 | 0 |
| لون45 | 255 | 153 | 0 |
| لون46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | بنية اللون. |
| الفهرس | int | فهرس لوحة الألوان، 0 - 55. |

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


يغلق الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). خيارات الوصول إلى البيانات |

### combine(Workbook secondWorkbook) {#combine-com.aspose.cells.Workbook-}
```
public void combine(Workbook secondWorkbook)
```


يجمع كائن دفتر عمل آخر.

**Remarks**

دمج ملفات Excel و ODS و CSV وغيرها في ملف واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| secondWorkbook | [Workbook](../../com.aspose.cells/workbook) | كائن دفتر عمل آخر. |

### copy(Workbook source) {#copy-com.aspose.cells.Workbook-}
```
public void copy(Workbook source)
```


ينسخ البيانات من كائن دفتر عمل المصدر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | كائن دفتر عمل المصدر. |

### copy(Workbook source, CopyOptions copyOptions) {#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-}
```
public void copy(Workbook source, CopyOptions copyOptions)
```


ينسخ كائن دفتر عمل آخر.

**Remarks**

من السهل جدًا استنساخ ملف Excel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | كائن دفتر عمل المصدر. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | خيارات نسخ دفتر عمل آخر. |

### copyTheme(Workbook source) {#copyTheme-com.aspose.cells.Workbook-}
```
public void copyTheme(Workbook source)
```


ينسخ السمة من دفتر عمل آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | دفتر عمل المصدر. |

### createBuiltinStyle(int type) {#createBuiltinStyle-int-}
```
public Style createBuiltinStyle(int type)
```


ينشئ نمطًا مدمجًا حسب النوع المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [BuiltinStyleType](../../com.aspose.cells/builtinstyletype). النمط المدمج. |

**Returns:**
[Style](../../com.aspose.cells/style) - [Style](../../com.aspose.cells/style) object
### createCellsColor() {#createCellsColor--}
```
public CellsColor createCellsColor()
```


ينشئ كائنًا من نوع [CellsColor](../../com.aspose.cells/cellscolor).

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor) - Returns a [CellsColor](../../com.aspose.cells/cellscolor) object.
### createStyle() {#createStyle--}
```
public Style createStyle()
```


ينشئ نمطًا جديدًا.

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### createStyle(boolean cloneDefaultStyle) {#createStyle-boolean-}
```
public Style createStyle(boolean cloneDefaultStyle)
```


ينشئ نمطًا جديدًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cloneDefaultStyle | boolean | يشير إلى ما إذا كان ينسخ النمط الافتراضي |

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### customTheme(String themeName, Color[] colors) {#customTheme-java.lang.String-com.aspose.cells.Color---}
```
public void customTheme(String themeName, Color[] colors)
```


يخصص السمة.

**Remarks**

يجب أن يكون طول الألوان 12.

| فهرس المصفوفة | نوع السمة |
| ----------- | ------------------ |
| 0 | الخلفية1 |
| 1 | نص1 |
| 2 | الخلفية2 |
| 3 | نص2 |
| 4 | تسليط1 |
| 5 | تسليط2 |
| 6 | تسليط3 |
| 7 | تسليط4 |
| 8 | تسليط5 |
| 9 | تسليط6 |
| 10 | ارتباط تشعبي |
| 11 | ارتباط تشعبي متابع |

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| themeName | java.lang.String | اسم السمة |
| colors | [Color\[\]](../../com.aspose.cells/color) | ألوان السمة |

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
### exportXml(String mapName, OutputStream stream) {#exportXml-java.lang.String-java.io.OutputStream-}
```
public void exportXml(String mapName, OutputStream stream)
```


يصدّر بيانات XML المرتبطة بخريطة XML المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| mapName | java.lang.String | اسم خريطة XML التي تحتاج إلى تصديرها |
| stream | java.io.OutputStream | دفق التصدير |

### exportXml(String mapName, String path) {#exportXml-java.lang.String-java.lang.String-}
```
public void exportXml(String mapName, String path)
```


يصدّر بيانات XML المرتبطة بخريطة XML المحددة.

**Example**

الكود التالي يصدر البيانات المرتبطة بأول XmlMap.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         //Make sure that the source xlsx file contains a XmlMap.
         XmlMap xmlMap = wb.getWorksheets().getXmlMaps().get(0);
 
         wb.exportXml(xmlMap.getName(), "output.xml");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| mapName | java.lang.String | اسم خريطة XML التي تحتاج إلى تصديرها |
| المسار | java.lang.String | مسار التصدير |

### getAbsolutePath() {#getAbsolutePath--}
```
public String getAbsolutePath()
```


يحصل على المسار المطلق للملف.

**Remarks**

يُستخدم فقط للروابط الخارجية.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


يرجع مجموعة [DocumentProperty](../../com.aspose.cells/documentproperty) تمثل جميع خصائص المستند المدمجة في جدول البيانات.

**Remarks**

لا يمكن إضافة خاصية جديدة إلى قائمة خصائص المستند المدمجة. يمكنك فقط الحصول على خاصية مدمجة وتغيير قيمتها. القائمة التالية هي أسماء الخصائص المدمجة:

Title

الموضوع

المؤلف

الكلمات المفتاحية

التعليقات

القالب

المؤلف الأخير

رقم المراجعة

اسم التطبيق

تاريخ الطباعة الأخير

تاريخ الإنشاء

وقت الحفظ الأخير

إجمالي وقت التحرير

عدد الصفحات

عدد الكلمات

عدد الأحرف

الأمان

الفئة

التنسيق

المدير

الشركة

عدد البايتات

عدد الأسطر

عدد الفقرات

عدد الشرائح

عدد الملاحظات

عدد الشرائح المخفية

عدد مقاطع الوسائط المتعددة

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getCellsDataTableFactory() {#getCellsDataTableFactory--}
```
public CellsDataTableFactory getCellsDataTableFactory()
```


يحصل على المصنع لبناء ICellsDataTable من كائنات مخصصة

**Returns:**
[CellsDataTableFactory](../../com.aspose.cells/cellsdatatablefactory)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColors() {#getColors--}
```
public Color[] getColors()
```


يعيد الألوان في لوحة الألوان لجدول البيانات.

**Remarks**

تحتوي اللوحة على 56 مدخلاً، كل منها ممثل بقيمة RGB.

**Returns:**
com.aspose.cells.Color[]
### getContentTypeProperties() {#getContentTypeProperties--}
```
public ContentTypePropertyCollection getContentTypeProperties()
```


يحصل على قائمة كائنات [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) في دفتر العمل.

**Returns:**
[ContentTypePropertyCollection](../../com.aspose.cells/contenttypepropertycollection)
### getCountOfStylesInPool() {#getCountOfStylesInPool--}
```
public int getCountOfStylesInPool()
```


يحصل على عدد الأنماط في مجموعة الأنماط.

**Returns:**
int
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


يرجع مجموعة [DocumentProperty](../../com.aspose.cells/documentproperty) تمثل جميع خصائص المستند المخصصة في جدول البيانات.

**Example**

```
         Workbook excel = new Workbook();
         excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getCustomXmlParts() {#getCustomXmlParts--}
```
public CustomXmlPartCollection getCustomXmlParts()
```


يمثل Custom XML Data Storage Part (بيانات XML مخصصة داخل حزمة).

**Returns:**
[CustomXmlPartCollection](../../com.aspose.cells/customxmlpartcollection)
### getDataConnections() {#getDataConnections--}
```
public ExternalConnectionCollection getDataConnections()
```


يحصل على مجموعة [ExternalConnection](../../com.aspose.cells/externalconnection).

**Returns:**
[ExternalConnectionCollection](../../com.aspose.cells/externalconnectioncollection)
### getDataMashup() {#getDataMashup--}
```
public DataMashup getDataMashup()
```


يحصل على بيانات الدمج.

**Returns:**
[DataMashup](../../com.aspose.cells/datamashup)
### getDataModel() {#getDataModel--}
```
public DataModel getDataModel()
```


يحصل على نموذج البيانات في دفتر العمل.

**Returns:**
[DataModel](../../com.aspose.cells/datamodel)
### getDataSorter() {#getDataSorter--}
```
public DataSorter getDataSorter()
```


يحصل على كائن DataSorter لفرز البيانات.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### getDefaultStyle() {#getDefaultStyle--}
```
public Style getDefaultStyle()
```


يحصل على كائن [Style](../../com.aspose.cells/style) الافتراضي لدفتر العمل.

**Remarks**

خاصية DefaultStyle مفيدة لتطبيق نمط على كامل Workbook.

**Example**

الكود التالي ينشئ ويُنشئ نسخة من Workbook جديد ويضبط [Style](../../com.aspose.cells/style) افتراضيًا له.

```
         Workbook workbook = new Workbook();
         Style defaultStyle = workbook.getDefaultStyle();
         defaultStyle.getFont().setName("Tahoma");
         workbook.setDefaultStyle(defaultStyle);
```

**Returns:**
[Style](../../com.aspose.cells/style)
### getDigitalSignature() {#getDigitalSignature--}
```
public DigitalSignatureCollection getDigitalSignature()
```


يحصل على التوقيع الرقمي من الملف.

**Returns:**
[DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


يحصل على تنسيق الملف.

انظر [FileFormatType](../../com.aspose.cells/fileformattype).

**Returns:**
int
### getFileName() {#getFileName--}
```
public String getFileName()
```


يحصل على اسم الملف الحالي.

**Remarks**

إذا تم فتح الملف عبر الدفق وكان هناك بعض مراجع الصيغ الخارجية، يرجى تعيين اسم الملف.

**Returns:**
java.lang.String
### getFonts() {#getFonts--}
```
public Font[] getFonts()
```


يحصل على جميع الخطوط في مجموعة الأنماط.

**Returns:**
com.aspose.cells.Font[]
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


يحصل على مراقب المقاطعة.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getMatchingColor(Color rawColor) {#getMatchingColor-com.aspose.cells.Color-}
```
public Color getMatchingColor(Color rawColor)
```


ابحث عن اللون الأنسب في لوحة الألوان الحالية.

**Remarks**

هناك فقط 56 لونًا في لوحة الألوان في Excel 97-2003. إذا لم يكن اللون موجودًا في اللوحة، سيتم تعيين اللون المشابه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rawColor | [Color](../../com.aspose.cells/color) | لون خام. |

**Returns:**
[Color](../../com.aspose.cells/color) - Best matching color.
### getNamedStyle(String name) {#getNamedStyle-java.lang.String-}
```
public Style getNamedStyle(String name)
```


يحصل على النمط المسمى في مجموعة الأنماط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم النمط. |

**Returns:**
[Style](../../com.aspose.cells/style) - named style, maybe null.
### getRibbonXml() {#getRibbonXml--}
```
public String getRibbonXml()
```


يحصل على ملف XML الذي يحدد واجهة الشريط.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public WorkbookSettings getSettings()
```


يمثل إعدادات المصنف.

**Returns:**
[WorkbookSettings](../../com.aspose.cells/workbooksettings)
### getStyleInPool(int index) {#getStyleInPool-int-}
```
public Style getStyleInPool(int index)
```


يحصل على النمط في مجموعة الأنماط. سيتم جمع جميع الأنماط في المصنف في مجموعة. هناك فقط فهرس إشارة بسيط في الخلايا.

**Remarks**

إذا تم تغيير النمط المرتجع، سيتغير نمط جميع الخلايا (التي تشير إلى هذا النمط).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

**Returns:**
[Style](../../com.aspose.cells/style) - The style in the pool corresponds to given index, may be null.
### getTheme() {#getTheme--}
```
public String getTheme()
```


يحصل على اسم السمة.

**Returns:**
java.lang.String
### getThemeColor(int type) {#getThemeColor-int-}
```
public Color getThemeColor(int type)
```


يحصل على لون السمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). نوع لون السمة. |

**Returns:**
[Color](../../com.aspose.cells/color) - The theme color.
### getVbaProject() {#getVbaProject--}
```
public VbaProject getVbaProject()
```


يحصل على [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) في جدول بيانات.

**Returns:**
[VbaProject](../../com.aspose.cells/vbaproject)
### getWorksheets() {#getWorksheets--}
```
public WorksheetCollection getWorksheets()
```


يحصل على مجموعة [WorksheetCollection](../../com.aspose.cells/worksheetcollection) في جدول البيانات.

**Returns:**
[WorksheetCollection](../../com.aspose.cells/worksheetcollection) - [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


يكشف ما إذا كان هناك دالة مخصصة مستخدمة في هذا المصنف، مثل في صيغة الخلية، أو في الأسماء المعرفة...

**Returns:**
boolean
### hasExernalLinks() {#hasExernalLinks--}
```
public boolean hasExernalLinks()
```


يشير إلى ما إذا كان هذا المصنف يحتوي على روابط خارجية لمصادر بيانات أخرى.

**Remarks**

ملاحظة: هذه العضوية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام ExternalLinkCollection.Count للتحقق مما إذا كان هناك روابط خارجية في هذا المصنف. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2021. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
منطقي - ما إذا كان هذا المصنف يحتوي على روابط خارجية إلى مصادر بيانات أخرى.
### hasMacro() {#hasMacro--}
```
public boolean hasMacro()
```


يشير إلى ما إذا كان هذا جدول البيانات يحتوي على ماكرو/VBA.

**Returns:**
boolean
### hasRevisions() {#hasRevisions--}
```
public boolean hasRevisions()
```


يحصل على ما إذا كان المصنف يحتوي على أي تغييرات متتبعة

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importXml(InputStream stream, String sheetName, int row, int col) {#importXml-java.io.InputStream-java.lang.String-int-int-}
```
public void importXml(InputStream stream, String sheetName, int row, int col)
```


يستورد/يحدّث ملف بيانات XML إلى المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق ملف XML. |
| sheetName | java.lang.String | اسم ورقة الوجهة. |
| صف | int | صف الوجهة. |
| col | int | عمود الوجهة. |

### importXml(String url, String sheetName, int row, int col) {#importXml-java.lang.String-java.lang.String-int-int-}
```
public void importXml(String url, String sheetName, int row, int col)
```


يستورد/يحدّث ملف بيانات XML إلى المصنف.

**Example**

الكود التالي يستورد بيانات XML إلى ورقة العمل 'Sheet 1' في الخلية A1.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         wb.importXml("xml.xml", "Sheet1", 0, 0);
 
         wb.save("output.xlsx");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عنوان URL | java.lang.String | عنوان URL/المسار لملف XML. |
| sheetName | java.lang.String | اسم ورقة الوجهة. |
| صف | int | صف الوجهة |
| col | int | عمود الوجهة |

### isColorInPalette(Color color) {#isColorInPalette-com.aspose.cells.Color-}
```
public boolean isColorInPalette(Color color)
```


يتحقق مما إذا كان اللون موجودًا في لوحة ألوان جدول البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | بنية اللون. |

**Returns:**
منطقي - يُرجع true إذا كان هذا اللون موجودًا في لوحة الألوان. وإلا، يُرجع false
### isDigitallySigned() {#isDigitallySigned--}
```
public boolean isDigitallySigned()
```


يشير إلى ما إذا كان هذا جدول البيانات موقعًا رقمياً.

**Returns:**
boolean
### isLicensed() {#isLicensed--}
```
public boolean isLicensed()
```


يشير إلى ما إذا تم تعيين الترخيص.

**Returns:**
boolean
### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}
```
public boolean isWorkbookProtectedWithPassword()
```


يشير إلى ما إذا كان الهيكل أو النافذة محميين بكلمة مرور.

**Returns:**
boolean
### mergeNamedStyles(Workbook source) {#mergeNamedStyles-com.aspose.cells.Workbook-}
```
public void mergeNamedStyles(Workbook source)
```


يدمج الأنماط المسمية من ملف Excel الآخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | الملف الآخر |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFormulas(boolean ignoreError) {#parseFormulas-boolean-}
```
public void parseFormulas(boolean ignoreError)
```


يفكّ تحليل جميع الصيغ التي لم يتم تحليلها عندما تم تحميلها من ملف القالب أو تعيينها إلى خلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ignoreError | boolean | ما إذا كان يجب تجاهل الخطأ للمعادلة غير الصالحة. بالنسبة لمعادلة غير صالحة واحدة، إذا تم تجاهل الخطأ فسيتم تجاهل هذه المعادلة وسيستمر العملية في تحليل المعادلات الأخرى، وإلا سيتم رمي استثناء. |

### protect(int protectionType, String password) {#protect-int-java.lang.String-}
```
public void protect(int protectionType, String password)
```


يحمي مصنفًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| protectionType | int | [ProtectionType](../../com.aspose.cells/protectiontype). نوع الحماية. |
| password | java.lang.String | كلمة المرور لحماية المصنف. |

### protectSharedWorkbook(String password) {#protectSharedWorkbook-java.lang.String-}
```
public void protectSharedWorkbook(String password)
```


يحمي مصنفًا مشتركًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| password | java.lang.String | كلمة المرور لحماية المصنف. |

### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


تحديث الأشكال المرتبطة، وجميع جداول المحور والرسوم البيانية بمصدر المحور.

### refreshDynamicArrayFormulas(boolean calculate) {#refreshDynamicArrayFormulas-boolean-}
```
public void refreshDynamicArrayFormulas(boolean calculate)
```


يقوم بتحديث صيغ المصفوفة الديناميكية (تنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية) لن يتم حساب الصيغ الأخرى في المصنف بشكل متكرر حتى إذا تم استخدامها بواسطة صيغ المصفوفة الديناميكية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| احسب | boolean | ما إذا كان يحسب ويحدّث قيم الخلايا لتلك المعادلات الديناميكية للمصفوفة |

### refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts) {#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-}
```
public void refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)
```


يقوم بتحديث صيغ المصفوفة الديناميكية (تنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية)

**Remarks**

لأسباب تتعلق بالأداء، لا نقوم بتحديث جميع معادلات المصفوفة الديناميكية تلقائيًا عندما تتغير المعادلة نفسها أو البيانات التي تشير إليها. لذا يحتاج المستخدم إلى استدعاء هذه الطريقة يدويًا بعد تلك العمليات التي قد تؤثر على معادلات المصفوفة الديناميكية، مثل استيراد/تعيين قيم الخلايا، إدراج/حذف الصفوف/الأعمدة/النطاقات، ... إلخ.

بالنسبة لمعظم المعادلات التي تحتوي على دوال، حساب نطاق الانسكاب يتطلب أيضًا حساب المعادلة، لذا يُفضَّل عمومًا قيمة true لعلامة "calculate". إذا كانت المعادلة بسيطة، مثل إشارة إلى نطاق أو مصفوفة (على سبيل المثال "=C1:E5", "=\{1,2;3,4\}", ...)، دالة بسيطة على نطاق أو مصفوفة (على سبيل المثال "=ABS(C1:E5)", "=1+\{1,2;3,4\}", ...)، وسيتم حساب جميع المعادلات لاحقًا (مثلًا عبر [calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-))، فإن استخدام قيمة false لعلامة "calculate" قد يتجنب الحساب المكرر لفائدة الأداء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| احسب | boolean | ما إذا كان يحسب ويحدّث قيم الخلايا لتلك المعادلات الديناميكية للمصفوفة |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | الخيارات لحساب المعادلات |

### removeDigitalSignature() {#removeDigitalSignature--}
```
public void removeDigitalSignature()
```


إزالة التوقيع الرقمي من هذه الورقة.

### removeExternalLinks() {#removeExternalLinks--}
```
public void removeExternalLinks()
```


إزالة جميع الروابط الخارجية في المصنف.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طريقة ExternalLinkCollection.Clear(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2021. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### removeMacro() {#removeMacro--}
```
public void removeMacro()
```


إزالة VBA/ماكرو من هذه الورقة.

### removePersonalInformation() {#removePersonalInformation--}
```
public void removePersonalInformation()
```


إزالة المعلومات الشخصية.

### removeUnusedStyles() {#removeUnusedStyles--}
```
public void removeUnusedStyles()
```


إزالة جميع الأنماط غير المستخدمة.

### replace(boolean boolValue, Object newValue) {#replace-boolean-java.lang.Object-}
```
public int replace(boolean boolValue, Object newValue)
```


استبدال قيم الخلايا ببيانات جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| boolValue | boolean | القيمة المنطقية التي سيتم استبدالها. |
| newValue | java.lang.Object | قيمة جديدة. يمكن أن تكون سلسلة، عدد صحيح، مزدوج أو قيمة DateTime. |

**Returns:**
int
### replace(int intValue, Object newValue) {#replace-int-java.lang.Object-}
```
public int replace(int intValue, Object newValue)
```


استبدال قيم الخلايا ببيانات جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| intValue | int | القيمة الصحيحة التي سيتم استبدالها. |
| newValue | java.lang.Object | قيمة جديدة. يمكن أن تكون سلسلة، عدد صحيح، مزدوج أو قيمة DateTime. |

**Returns:**
int
### replace(String placeHolder, double newValue) {#replace-java.lang.String-double-}
```
public int replace(String placeHolder, double newValue)
```


استبدال قيمة خلية واحدة بعدد مزدوج جديد.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double newValue = 100.0;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | java.lang.String | عنصر نائب للخلية |
| newValue | double | قيمة مزدوجة للاستبدال |

**Returns:**
int
### replace(String placeHolder, double[] newValues, boolean isVertical) {#replace-java.lang.String-double---boolean-}
```
public int replace(String placeHolder, double[] newValues, boolean isVertical)
```


استبدال قيم الخلايا بمصفوفة مزدوجة.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double[] newValues = new double[]{1.23, 2.56, 3.14159};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | java.lang.String | عنصر نائب للخلية |
| newValues | double[] | مصفوفة مزدوجة للاستبدال |
| isVertical | boolean | صحيح - عمودي، خطأ - أفقي |

**Returns:**
int
### replace(String placeHolder, int newValue) {#replace-java.lang.String-int-}
```
public int replace(String placeHolder, int newValue)
```


استبدال قيمة خلية واحدة بعدد صحيح جديد.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int newValue = 100;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | java.lang.String | عنصر نائب للخلية |
| newValue | int | قيمة عدد صحيح للاستبدال |

**Returns:**
int
### replace(String placeHolder, int[] newValues, boolean isVertical) {#replace-java.lang.String-int---boolean-}
```
public int replace(String placeHolder, int[] newValues, boolean isVertical)
```


استبدال قيم الخلايا بمصفوفة أعداد صحيحة.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int[] newValues = new int[]{1, 2, 3};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | java.lang.String | عنصر نائب للخلية |
| newValues | int[] | مصفوفة أعداد صحيحة للاستبدال |
| isVertical | boolean | صحيح - عمودي، خطأ - أفقي |

**Returns:**
int
### replace(String placeHolder, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String placeHolder, String newValue)
```


استبدال قيمة خلية واحدة بسلسلة نصية جديدة.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         workbook.replace("AnOldValue", "NewValue");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | java.lang.String | عنصر نائب للخلية |
| newValue | java.lang.String | قيمة سلسلة للاستبدال |

**Returns:**
int
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public int replace(String placeHolder, String newValue, ReplaceOptions options)
```


استبدال قيمة خلية واحدة بسلسلة نصية جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | java.lang.String | عنصر نائب للخلية |
| newValue | java.lang.String | قيمة سلسلة للاستبدال |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | خيارات الاستبدال |

**Returns:**
int
### replace(String placeHolder, String[] newValues, boolean isVertical) {#replace-java.lang.String-java.lang.String---boolean-}
```
public int replace(String placeHolder, String[] newValues, boolean isVertical)
```


استبدال قيمة خلية واحدة بمصفوفة سلاسل نصية جديدة.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         String[] newValues = new String[]{"Tom", "Alice", "Jerry"};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | java.lang.String | عنصر نائب للخلية |
| newValues | java.lang.String[] | مصفوفة سلاسل للاستبدال |
| isVertical | boolean | صحيح - عمودي، خطأ - أفقي |

**Returns:**
int
### save(OutputStream stream, SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.cells.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions saveOptions)
```


حفظ المصنف إلى الدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الملف. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | خيارات الحفظ. |

### save(OutputStream stream, int saveFormat) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int saveFormat)
```


حفظ المصنف إلى الدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الملف. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). نوع تنسيق ملف الحفظ. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


حفظ المصنف إلى القرص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String |  |

### save(String fileName, SaveOptions saveOptions) {#save-java.lang.String-com.aspose.cells.SaveOptions-}
```
public void save(String fileName, SaveOptions saveOptions)
```


يحفظ المصنف إلى القرص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | خيارات الحفظ. |

### save(String fileName, int saveFormat) {#save-java.lang.String-int-}
```
public void save(String fileName, int saveFormat)
```


يحفظ المصنف إلى القرص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). نوع تنسيق الحفظ. |

### setAbsolutePath(String value) {#setAbsolutePath-java.lang.String-}
```
public void setAbsolutePath(String value)
```


تعيين المسار المطلق للملف.

**Remarks**

يُستخدم فقط للروابط الخارجية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDefaultStyle(Style value) {#setDefaultStyle-com.aspose.cells.Style-}
```
public void setDefaultStyle(Style value)
```


تعيين كائن [Style](../../com.aspose.cells/style) الافتراضي للمصنف.

**Remarks**

خاصية DefaultStyle مفيدة لتطبيق نمط على كامل Workbook.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


تعيين توقيع رقمي لملف ورقة عمل (Excel2007 وما بعده).

**Remarks**

يدعم فقط إضافة توقيع رقمي Xmldsig

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### setEncryptionOptions(int encryptionType, int keyLength) {#setEncryptionOptions-int-int-}
```
public void setEncryptionOptions(int encryptionType, int keyLength)
```


تعيين خيارات التشفير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| encryptionType | int | [EncryptionType](../../com.aspose.cells/encryptiontype). نوع التشفير. |
| keyLength | int | طول المفتاح. |

### setFileFormat(int value) {#setFileFormat-int-}
```
public void setFileFormat(int value)
```


تعيين تنسيق الملف.

انظر [FileFormatType](../../com.aspose.cells/fileformattype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFileName(String value) {#setFileName-java.lang.String-}
```
public void setFileName(String value)
```


تعيين اسم الملف الحالي.

**Remarks**

إذا تم فتح الملف عبر الدفق وكان هناك بعض مراجع الصيغ الخارجية، يرجى تعيين اسم الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


يضبط مراقب المقاطعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setRibbonXml(String value) {#setRibbonXml-java.lang.String-}
```
public void setRibbonXml(String value)
```


تعيين ملف XML الذي يحدد واجهة شريط الأدوات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setThemeColor(int type, Color color) {#setThemeColor-int-com.aspose.cells.Color-}
```
public void setThemeColor(int type, Color color)
```


يضبط لون السمة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). نوع لون السمة. |
| color | [Color](../../com.aspose.cells/color) | لون السمة |

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


يبدأ الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات.

**Remarks**

إذا كان ذاكرة التخزين المؤقت للوصول إلى البيانات المحددة تتطلب أن تكون بعض نماذج البيانات في ورقة العمل "للقراءة فقط"، فسيتم اعتبار نماذج البيانات المقابلة في كل ورقة عمل في هذا المصنف "للقراءة فقط" ويجب على المستخدم عدم تغيير أي منها.

بعد الانتهاء من الوصول إلى البيانات، يجب استدعاء [closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-) بنفس الخيارات لمسح جميع الذاكرات المؤقتة واستعادة وضع الوصول العادي.



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). خيارات الوصول إلى البيانات |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


يفك حماية مصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| password | java.lang.String | كلمة المرور لإلغاء حماية المصنف. |

### unprotectSharedWorkbook(String password) {#unprotectSharedWorkbook-java.lang.String-}
```
public void unprotectSharedWorkbook(String password)
```


يفك حماية مصنف مشترك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| password | java.lang.String | كلمة المرور لإلغاء حماية المصنف. |

### updateCustomFunctionDefinition(CustomFunctionDefinition definition) {#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void updateCustomFunctionDefinition(CustomFunctionDefinition definition)
```


يحدّث تعريف الدوال المخصصة.

**Remarks**

يمكن استخدام هذه الطريقة لبعض السيناريوهات الخاصة. على سبيل المثال، إذا كان المستخدم يحتاج إلى حساب بعض معلمات بعض الدوال المخصصة في وضع المصفوفة، يمكن للمستخدم توفير تعريفه الخاص مع تنفيذ [CustomFunctionDefinition.getArrayModeParameters(String)](../../com.aspose.cells/customfunctiondefinition\#getArrayModeParameters-String-) لتلك الدوال. بعد تحديث بيانات الصيغ، سيتم حساب تلك المعلمات المحددة في وضع المصفوفة تلقائيًا عند حساب الدوال المخصصة المقابلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| definition | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) | تعريف خاص للدوال المخصصة لتلبية متطلبات المستخدم الخاصة. |

### updateLinkedDataSource(Workbook[] externalWorkbooks) {#updateLinkedDataSource-com.aspose.cells.Workbook---}
```
public void updateLinkedDataSource(Workbook[] externalWorkbooks)
```


إذا كان هذا المصنف يحتوي على روابط خارجية إلى مصدر بيانات آخر، سيحاول Aspose.Cells استرجاع أحدث البيانات من المصادر المعطاة.

**Remarks**

إذا تعذر العثور على الرابط الخارجي المقابل لأحد المصنفات، فسيتم تجاهل هذا المصنف. لذلك عندما تقوم بتعيين صيغة لاحقًا باستخدام رابط خارجي جديد ترغب في ربط المصنف المتجاهل به، لا يمكن تنفيذ الربط حتى تستدعي هذه الطريقة مرة أخرى مع تلك المصنفات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| externalWorkbooks | [Workbook\[\]](../../com.aspose.cells/workbook) | المصنفات التي ستُستخدم لتحديث بيانات الروابط الخارجية المشار إليها من قبل هذا المصنف. يتم تحديد مطابقة تلك المصنفات مع الروابط الخارجية بواسطة [getFileName()](../../com.aspose.cells/workbook\#getFileName--) و[ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). لذا يرجى التأكد من أن [getFileName()](../../com.aspose.cells/workbook\#getFileName--) تم تحديده بالقيمة المناسبة لكل مصنف حتى يمكن ربطه بالرابط الخارجي المقابل. |

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

