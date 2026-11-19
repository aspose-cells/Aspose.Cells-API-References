---
title: "PageSetup"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل وصف إعداد الصفحة."
type: docs
url: /ar/java/com.aspose.cells/pagesetup/
---

**Inheritance:**
java.lang.Object
```
public class PageSetup
```

يحتوي على الكائن الذي يمثل وصف إعداد الصفحة. يحتوي كائن PageSetup على جميع خيارات إعداد الصفحة.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
         Worksheet sheet = sheets.get(1);
         PageSetup pageSetup = sheet.getPageSetup();
         pageSetup.setPrintArea("D1:K13");
 
         //do your business
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [clearHeaderFooter()](#clearHeaderFooter--) | يمسح إعدادات الرأس والتذييل. |
| [copy(PageSetup source, CopyOptions copyOptions)](#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-) | ينسخ إعدادات إعداد الصفحة. |
| [customPaperSize(double width, double height)](#customPaperSize-double-double-) | يضبط حجم الورق المخصص، بوحدة البوصة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBlackAndWhite()](#getBlackAndWhite--) | يمثل ما إذا كانت عناصر المستند ستُطبع بالأبيض والأسود. |
| [getBottomMargin()](#getBottomMargin--) | يمثل حجم الهامش السفلي، بوحدة السنتيمتر. |
| [getBottomMarginInch()](#getBottomMarginInch--) | يمثل حجم الهامش السفلي، بوحدة البوصة. |
| [getCenterHorizontally()](#getCenterHorizontally--) | يمثل ما إذا كانت الورقة تُطبع متمركزة أفقياً. |
| [getCenterVertically()](#getCenterVertically--) | يمثل ما إذا كانت الورقة تُطبع متمركزة عمودياً. |
| [getClass()](#getClass--) |  |
| [getCommands(String headerFooterScript)](#getCommands-java.lang.String-) | يحصل على جميع أوامر الرأس أو التذييل. |
| [getEvenFooter(int section)](#getEvenFooter-int-) | يحصل على برنامج نصي ينسق التذييل الزوجي لملف إكسل. |
| [getEvenHeader(int section)](#getEvenHeader-int-) | يحصل على برنامج نصي ينسق الرأس الزوجي لملف إكسل. |
| [getFirstPageFooter(int section)](#getFirstPageFooter-int-) | يحصل على برنامج نصي ينسق تذييل الصفحة الأولى لملف إكسل. |
| [getFirstPageHeader(int section)](#getFirstPageHeader-int-) | يحصل على برنامج نصي ينسق رأس الصفحة الأولى لملف إكسل. |
| [getFirstPageNumber()](#getFirstPageNumber--) | يمثل رقم الصفحة الأولى الذي سيُستخدم عند طباعة هذه الورقة. |
| [getFitToPagesTall()](#getFitToPagesTall--) | يمثل عدد الصفحات في الارتفاع التي سيتم تحجيم الورقة إليها عند طباعتها. |
| [getFitToPagesWide()](#getFitToPagesWide--) | يمثل عدد الصفحات في العرض التي سيتم تحجيم الورقة إليها عند طباعتها. |
| [getFooter(int section)](#getFooter-int-) | يحصل على برنامج نصي ينسق التذييل لملف إكسل. |
| [getFooterMargin()](#getFooterMargin--) | يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة السنتيمتر. |
| [getFooterMarginInch()](#getFooterMarginInch--) | يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة البوصة. |
| [getHeader(int section)](#getHeader-int-) | يحصل على برنامج نصي ينسق الرأس لملف إكسل. |
| [getHeaderMargin()](#getHeaderMargin--) | يمثل المسافة من أعلى الصفحة إلى الرأس، بوحدة السنتيمتر. |
| [getHeaderMarginInch()](#getHeaderMarginInch--) | يمثل المسافة من أعلى الصفحة إلى الرأس، بوحدة البوصة. |
| [getLeftMargin()](#getLeftMargin--) | يمثل حجم الهامش الأيسر، بوحدة السنتيمتر. |
| [getLeftMarginInch()](#getLeftMarginInch--) | يمثل حجم الهامش الأيسر، بوحدة البوصة. |
| [getODSPageBackground()](#getODSPageBackground--) | يحصل على خلفية ODS. |
| [getOrder()](#getOrder--) | يمثل الترتيب الذي يستخدمه Microsoft Excel لترقيم الصفحات عند طباعة ورقة عمل كبيرة. |
| [getOrientation()](#getOrientation--) | يمثل اتجاه طباعة الصفحة. |
| [getPaperHeight()](#getPaperHeight--) | يحصل على ارتفاع الورق بوحدة البوصة، مع اعتبار اتجاه الصفحة. |
| [getPaperSize()](#getPaperSize--) | يمثل حجم الورق. |
| [getPaperWidth()](#getPaperWidth--) | يحصل على عرض الورق بوحدة البوصة، مع اعتبار اتجاه الصفحة. |
| [getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)](#getPicture-boolean-boolean-boolean-int-) | يحصل على كائن [Picture](../../com.aspose.cells/picture) للرأس / التذييل. |
| [getPicture(boolean isHeader, int section)](#getPicture-boolean-int-) | يحصل على كائن [Picture](../../com.aspose.cells/picture) للرأس / التذييل. |
| [getPrintArea()](#getPrintArea--) | يمثل النطاق الذي سيُطبع. |
| [getPrintComments()](#getPrintComments--) | يمثل طريقة طباعة التعليقات مع الورقة. |
| [getPrintCopies()](#getPrintCopies--) | يحصل على عدد النسخ للطباعة. |
| [getPrintDraft()](#getPrintDraft--) | يمثل ما إذا كان سيتم طباعة الورقة بدون رسومات. |
| [getPrintErrors()](#getPrintErrors--) | يحدد نوع خطأ الطباعة المعروض. |
| [getPrintGridlines()](#getPrintGridlines--) | يمثل ما إذا كانت خطوط الشبكة الخلوية مطبوعة على الصفحة. |
| [getPrintHeadings()](#getPrintHeadings--) | يمثل ما إذا كانت عناوين الصفوف والأعمدة مطبوعة مع هذه الصفحة. |
| [getPrintQuality()](#getPrintQuality--) | يمثل جودة الطباعة. |
| [getPrintTitleColumns()](#getPrintTitleColumns--) | يمثل الأعمدة التي تحتوي على الخلايا التي ستُعاد على الجانب الأيسر من كل صفحة. |
| [getPrintTitleRows()](#getPrintTitleRows--) | يمثل الصفوف التي تحتوي على الخلايا التي ستُعاد في أعلى كل صفحة. |
| [getPrinterSettings()](#getPrinterSettings--) | يحصل على إعدادات الطابعة الافتراضية. |
| [getRightMargin()](#getRightMargin--) | يمثل حجم الهامش الأيمن، بوحدة السنتيمترات. |
| [getRightMarginInch()](#getRightMarginInch--) | يمثل حجم الهامش الأيمن، بوحدة البوصات. |
| [getTopMargin()](#getTopMargin--) | يمثل حجم الهامش العلوي، بوحدة السنتيمترات. |
| [getTopMarginInch()](#getTopMarginInch--) | يمثل حجم الهامش العلوي، بوحدة البوصات. |
| [getZoom()](#getZoom--) | يمثل عامل التحجيم بالنسبة المئوية. |
| [hashCode()](#hashCode--) |  |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--) | يشير إلى ما إذا كان رقم الصفحة الأول يتم تعيينه تلقائيًا. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--) | يشير إلى ما إذا كان حجم الورق تلقائيًا. |
| [isHFAlignMargins()](#isHFAlignMargins--) | يشير إلى ما إذا كانت هوامش الرأس والتذييل محاذية مع هوامش الصفحة. |
| [isHFDiffFirst()](#isHFDiffFirst--) | صحيح يعني أن رأس/تذييل الصفحة الأولى مختلف عن الصفحات الأخرى. |
| [isHFDiffOddEven()](#isHFDiffOddEven--) | صحيح يعني أن رأس/تذييل الصفحات الفردية مختلف عن الصفحات الفردية. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--) | يشير إلى ما إذا كان يتم تحجيم الرأس والتذييل مع تحجيم المستند. |
| [isPercentScale()](#isPercentScale--) | إذا كانت هذه الخاصية خاطئة، فإن خاصيتي FitToPagesWide وFitToPagesTall تتحكمان في كيفية تحجيم ورقة العمل. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFirstPageNumber(boolean value)](#setAutoFirstPageNumber-boolean-) | يشير إلى ما إذا كان رقم الصفحة الأول يتم تعيينه تلقائيًا. |
| [setBlackAndWhite(boolean value)](#setBlackAndWhite-boolean-) | يمثل ما إذا كانت عناصر المستند ستُطبع بالأبيض والأسود. |
| [setBottomMargin(double value)](#setBottomMargin-double-) | يمثل حجم الهامش السفلي، بوحدة السنتيمتر. |
| [setBottomMarginInch(double value)](#setBottomMarginInch-double-) | يمثل حجم الهامش السفلي، بوحدة البوصة. |
| [setCenterHorizontally(boolean value)](#setCenterHorizontally-boolean-) | يمثل ما إذا كانت الورقة تُطبع متمركزة أفقياً. |
| [setCenterVertically(boolean value)](#setCenterVertically-boolean-) | يمثل ما إذا كانت الورقة تُطبع متمركزة عمودياً. |
| [setEvenFooter(int section, String footerScript)](#setEvenFooter-int-java.lang.String-) | يضبط برنامجًا نصيًا لتنسيق تذييل الصفحات الزوجية في ملف Excel. |
| [setEvenHeader(int section, String headerScript)](#setEvenHeader-int-java.lang.String-) | يضبط برنامجًا نصيًا لتنسيق رأس الصفحات الزوجية في ملف Excel. |
| [setFirstPageFooter(int section, String footerScript)](#setFirstPageFooter-int-java.lang.String-) | يضبط برنامجًا نصيًا لتنسيق تذييل الصفحة الأولى في ملف Excel. |
| [setFirstPageHeader(int section, String headerScript)](#setFirstPageHeader-int-java.lang.String-) | يضبط برنامجًا نصيًا لتنسيق رأس الصفحة الأولى في ملف Excel. |
| [setFirstPageNumber(int value)](#setFirstPageNumber-int-) | يمثل رقم الصفحة الأولى الذي سيُستخدم عند طباعة هذه الورقة. |
| [setFitToPages(int wide, int tall)](#setFitToPages-int-int-) | يضبط عدد الصفحات التي سيتم تحجيم ورقة العمل إليها عند طباعتها. |
| [setFitToPagesTall(int value)](#setFitToPagesTall-int-) | يمثل عدد الصفحات في الارتفاع التي سيتم تحجيم الورقة إليها عند طباعتها. |
| [setFitToPagesWide(int value)](#setFitToPagesWide-int-) | يمثل عدد الصفحات في العرض التي سيتم تحجيم الورقة إليها عند طباعتها. |
| [setFooter(int section, String footerScript)](#setFooter-int-java.lang.String-) | يضبط سكريبت لتنسيق تذييل ملف Excel. |
| [setFooterMargin(double value)](#setFooterMargin-double-) | يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة السنتيمتر. |
| [setFooterMarginInch(double value)](#setFooterMarginInch-double-) | يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة البوصة. |
| [setFooterPicture(int section, byte[] footerPicture)](#setFooterPicture-int-byte---) | يضبط صورة في تذييل ورقة العمل. |
| [setHFAlignMargins(boolean value)](#setHFAlignMargins-boolean-) | يشير إلى ما إذا كانت هوامش الرأس والتذييل محاذية مع هوامش الصفحة. |
| [setHFDiffFirst(boolean value)](#setHFDiffFirst-boolean-) | صحيح يعني أن رأس/تذييل الصفحة الأولى مختلف عن الصفحات الأخرى. |
| [setHFDiffOddEven(boolean value)](#setHFDiffOddEven-boolean-) | صحيح يعني أن رأس/تذييل الصفحات الفردية مختلف عن الصفحات الفردية. |
| [setHFScaleWithDoc(boolean value)](#setHFScaleWithDoc-boolean-) | يشير إلى ما إذا كان يتم تحجيم الرأس والتذييل مع تحجيم المستند. |
| [setHeader(int section, String headerScript)](#setHeader-int-java.lang.String-) | يضبط سكريبت لتنسيق رأس ملف Excel. |
| [setHeaderMargin(double value)](#setHeaderMargin-double-) | يمثل المسافة من أعلى الصفحة إلى الرأس، بوحدة السنتيمتر. |
| [setHeaderMarginInch(double value)](#setHeaderMarginInch-double-) | يمثل المسافة من أعلى الصفحة إلى الرأس، بوحدة البوصة. |
| [setHeaderPicture(int section, byte[] headerPicture)](#setHeaderPicture-int-byte---) | يضبط صورة في رأس ورقة العمل. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | يمثل حجم الهامش الأيسر، بوحدة السنتيمتر. |
| [setLeftMarginInch(double value)](#setLeftMarginInch-double-) | يمثل حجم الهامش الأيسر، بوحدة البوصة. |
| [setOrder(int value)](#setOrder-int-) | يمثل الترتيب الذي يستخدمه Microsoft Excel لترقيم الصفحات عند طباعة ورقة عمل كبيرة. |
| [setOrientation(int value)](#setOrientation-int-) | يمثل اتجاه طباعة الصفحة. |
| [setPaperSize(int value)](#setPaperSize-int-) | يمثل حجم الورق. |
| [setPercentScale(boolean value)](#setPercentScale-boolean-) | إذا كانت هذه الخاصية خاطئة، فإن خاصيتي FitToPagesWide وFitToPagesTall تتحكمان في كيفية تحجيم ورقة العمل. |
| [setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)](#setPicture-boolean-boolean-boolean-int-byte---) | يضبط صورة في رأس/تذييل ورقة العمل. |
| [setPrintArea(String value)](#setPrintArea-java.lang.String-) | يمثل النطاق الذي سيُطبع. |
| [setPrintComments(int value)](#setPrintComments-int-) | يمثل طريقة طباعة التعليقات مع الورقة. |
| [setPrintCopies(int value)](#setPrintCopies-int-) | يضبط عدد النسخ للطباعة. |
| [setPrintDraft(boolean value)](#setPrintDraft-boolean-) | يمثل ما إذا كان سيتم طباعة الورقة بدون رسومات. |
| [setPrintErrors(int value)](#setPrintErrors-int-) | يحدد نوع خطأ الطباعة المعروض. |
| [setPrintGridlines(boolean value)](#setPrintGridlines-boolean-) | يمثل ما إذا كانت خطوط الشبكة الخلوية مطبوعة على الصفحة. |
| [setPrintHeadings(boolean value)](#setPrintHeadings-boolean-) | يمثل ما إذا كانت عناوين الصفوف والأعمدة مطبوعة مع هذه الصفحة. |
| [setPrintQuality(int value)](#setPrintQuality-int-) | يمثل جودة الطباعة. |
| [setPrintTitleColumns(String value)](#setPrintTitleColumns-java.lang.String-) | يمثل الأعمدة التي تحتوي على الخلايا التي ستُعاد على الجانب الأيسر من كل صفحة. |
| [setPrintTitleRows(String value)](#setPrintTitleRows-java.lang.String-) | يمثل الصفوف التي تحتوي على الخلايا التي ستُعاد في أعلى كل صفحة. |
| [setPrinterSettings(byte[] value)](#setPrinterSettings-byte---) | يضبط إعدادات الطابعة الافتراضية. |
| [setRightMargin(double value)](#setRightMargin-double-) | يمثل حجم الهامش الأيمن، بوحدة السنتيمترات. |
| [setRightMarginInch(double value)](#setRightMarginInch-double-) | يمثل حجم الهامش الأيمن، بوحدة البوصات. |
| [setTopMargin(double value)](#setTopMargin-double-) | يمثل حجم الهامش العلوي، بوحدة السنتيمترات. |
| [setTopMarginInch(double value)](#setTopMarginInch-double-) | يمثل حجم الهامش العلوي، بوحدة البوصات. |
| [setZoom(int value)](#setZoom-int-) | يمثل عامل التحجيم بالنسبة المئوية. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clearHeaderFooter() {#clearHeaderFooter--}
```
public void clearHeaderFooter()
```


يمسح إعدادات الرأس والتذييل.

### copy(PageSetup source, CopyOptions copyOptions) {#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-}
```
public void copy(PageSetup source, CopyOptions copyOptions)
```


ينسخ إعدادات إعداد الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [PageSetup](../../com.aspose.cells/pagesetup) | المصدر. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | خيارات النسخ. |

### customPaperSize(double width, double height) {#customPaperSize-double-double-}
```
public void customPaperSize(double width, double height)
```


يضبط حجم الورق المخصص، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| العرض | double | عرض الورق. |
| الارتفاع | double | ارتفاع الورق. |

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
### getBlackAndWhite() {#getBlackAndWhite--}
```
public boolean getBlackAndWhite()
```


يمثل ما إذا كانت عناصر المستند ستُطبع بالأبيض والأسود.

**Returns:**
boolean
### getBottomMargin() {#getBottomMargin--}
```
public double getBottomMargin()
```


يمثل حجم الهامش السفلي، بوحدة السنتيمتر.

**Returns:**
double
### getBottomMarginInch() {#getBottomMarginInch--}
```
public double getBottomMarginInch()
```


يمثل حجم الهامش السفلي، بوحدة البوصة.

**Returns:**
double
### getCenterHorizontally() {#getCenterHorizontally--}
```
public boolean getCenterHorizontally()
```


يمثل ما إذا كانت الورقة تُطبع متمركزة أفقياً.

**Returns:**
boolean
### getCenterVertically() {#getCenterVertically--}
```
public boolean getCenterVertically()
```


يمثل ما إذا كانت الورقة تُطبع متمركزة عمودياً.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommands(String headerFooterScript) {#getCommands-java.lang.String-}
```
public HeaderFooterCommand[] getCommands(String headerFooterScript)
```


يحصل على جميع أوامر الرأس أو التذييل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| headerFooterScript | java.lang.String | سكريبت الرأس/التذييل |

**Returns:**
com.aspose.cells.HeaderFooterCommand[] - يرجع جميع أوامر الرأس أو التذييل.
### getEvenFooter(int section) {#getEvenFooter-int-}
```
public String getEvenFooter(int section)
```


يحصل على برنامج نصي ينسق التذييل الزوجي لملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

**Returns:**
java.lang.String
### getEvenHeader(int section) {#getEvenHeader-int-}
```
public String getEvenHeader(int section)
```


يحصل على برنامج نصي ينسق الرأس الزوجي لملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

**Returns:**
java.lang.String
### getFirstPageFooter(int section) {#getFirstPageFooter-int-}
```
public String getFirstPageFooter(int section)
```


يحصل على برنامج نصي ينسق تذييل الصفحة الأولى لملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

**Returns:**
java.lang.String
### getFirstPageHeader(int section) {#getFirstPageHeader-int-}
```
public String getFirstPageHeader(int section)
```


يحصل على برنامج نصي ينسق رأس الصفحة الأولى لملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

**Returns:**
java.lang.String
### getFirstPageNumber() {#getFirstPageNumber--}
```
public int getFirstPageNumber()
```


يمثل رقم الصفحة الأولى الذي سيُستخدم عند طباعة هذه الورقة.

**Returns:**
int
### getFitToPagesTall() {#getFitToPagesTall--}
```
public int getFitToPagesTall()
```


يمثل عدد الصفحات في الارتفاع التي سيتم تحجيم ورقة العمل إليها عند طباعتها. القيمة الافتراضية هي 1.

**Remarks**

يجب ضبط FitToPagesWide على الصفر إذا أردت ملاءمة جميع الصفوف في صفحة واحدة.

**Returns:**
int
### getFitToPagesWide() {#getFitToPagesWide--}
```
public int getFitToPagesWide()
```


يمثل عدد الصفحات في العرض التي سيتم تحجيم ورقة العمل إليها عند طباعتها. القيمة الافتراضية هي 1.

**Remarks**

يجب ضبط FitToPagesTall على الصفر إذا أردت ملاءمة جميع الأعمدة في صفحة واحدة.

**Returns:**
int
### getFooter(int section) {#getFooter-int-}
```
public String getFooter(int section)
```


يحصل على برنامج نصي ينسق التذييل لملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

**Returns:**
java.lang.String
### getFooterMargin() {#getFooterMargin--}
```
public double getFooterMargin()
```


يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة السنتيمتر.

**Returns:**
double
### getFooterMarginInch() {#getFooterMarginInch--}
```
public double getFooterMarginInch()
```


يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة البوصة.

**Returns:**
double
### getHeader(int section) {#getHeader-int-}
```
public String getHeader(int section)
```


يحصل على برنامج نصي ينسق الرأس لملف إكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

**Returns:**
java.lang.String
### getHeaderMargin() {#getHeaderMargin--}
```
public double getHeaderMargin()
```


يمثل المسافة من أعلى الصفحة إلى الرأس، بوحدة السنتيمتر.

**Returns:**
double
### getHeaderMarginInch() {#getHeaderMarginInch--}
```
public double getHeaderMarginInch()
```


يمثل المسافة من أعلى الصفحة إلى الرأس، بوحدة البوصة.

**Returns:**
double
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


يمثل حجم الهامش الأيسر، بوحدة السنتيمتر.

**Returns:**
double
### getLeftMarginInch() {#getLeftMarginInch--}
```
public double getLeftMarginInch()
```


يمثل حجم الهامش الأيسر، بوحدة البوصة.

**Returns:**
double
### getODSPageBackground() {#getODSPageBackground--}
```
public OdsPageBackground getODSPageBackground()
```


يحصل على خلفية ODS.

**Returns:**
[OdsPageBackground](../../com.aspose.cells/odspagebackground)
### getOrder() {#getOrder--}
```
public int getOrder()
```


يمثل الترتيب الذي يستخدمه Microsoft Excel لترقيم الصفحات عند طباعة ورقة عمل كبيرة.

انظر إلى [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


يمثل اتجاه طباعة الصفحة.

انظر [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Returns:**
int
### getPaperHeight() {#getPaperHeight--}
```
public double getPaperHeight()
```


يحصل على ارتفاع الورق بوحدة البوصة، مع اعتبار اتجاه الصفحة.

**Returns:**
double
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


يمثل حجم الورق.

انظر [PaperSizeType](../../com.aspose.cells/papersizetype).

**Returns:**
int
### getPaperWidth() {#getPaperWidth--}
```
public double getPaperWidth()
```


يحصل على عرض الورق بوحدة البوصة، مع اعتبار اتجاه الصفحة.

**Returns:**
double
### getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section) {#getPicture-boolean-boolean-boolean-int-}
```
public Picture getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)
```


يحصل على كائن [Picture](../../com.aspose.cells/picture) للرأس / التذييل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isFirst | boolean | يشير إلى ما إذا كان يتم الحصول على صورة رأس/تذييل الصفحة الأولى. |
| isEven | boolean | يشير إلى ما إذا كان يتم الحصول على صورة رأس/تذييل الصفحة الزوجية. |
| isHeader | boolean | يشير إلى ما إذا كان يتم الحصول على صورة الترويسة/التذييل. |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### getPicture(boolean isHeader, int section) {#getPicture-boolean-int-}
```
public Picture getPicture(boolean isHeader, int section)
```


يحصل على كائن [Picture](../../com.aspose.cells/picture) للرأس / التذييل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isHeader | boolean | يشير إلى ما إذا كان موجودًا في الترويسة أو التذييل. |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object. Returns null if there is no picture.
### getPrintArea() {#getPrintArea--}
```
public String getPrintArea()
```


يمثل النطاق الذي سيُطبع.

**Returns:**
java.lang.String
### getPrintComments() {#getPrintComments--}
```
public int getPrintComments()
```


يمثل طريقة طباعة التعليقات مع الورقة.

انظر [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getPrintCopies() {#getPrintCopies--}
```
public int getPrintCopies()
```


يحصل على عدد النسخ للطباعة.

**Returns:**
int
### getPrintDraft() {#getPrintDraft--}
```
public boolean getPrintDraft()
```


يمثل ما إذا كان سيتم طباعة الورقة بدون رسومات.

**Returns:**
boolean
### getPrintErrors() {#getPrintErrors--}
```
public int getPrintErrors()
```


يحدد نوع خطأ الطباعة المعروض.

انظر إلى [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Returns:**
int
### getPrintGridlines() {#getPrintGridlines--}
```
public boolean getPrintGridlines()
```


يمثل ما إذا كانت خطوط الشبكة الخلوية مطبوعة على الصفحة.

**Returns:**
boolean
### getPrintHeadings() {#getPrintHeadings--}
```
public boolean getPrintHeadings()
```


يمثل ما إذا كانت عناوين الصفوف والأعمدة مطبوعة مع هذه الصفحة.

**Returns:**
boolean
### getPrintQuality() {#getPrintQuality--}
```
public int getPrintQuality()
```


يمثل جودة الطباعة.

**Returns:**
int
### getPrintTitleColumns() {#getPrintTitleColumns--}
```
public String getPrintTitleColumns()
```


يمثل الأعمدة التي تحتوي على الخلايا التي ستُعاد على الجانب الأيسر من كل صفحة.

**Example**

```
         pageSetup.setPrintTitleColumns("$A:$A");
```

**Returns:**
java.lang.String
### getPrintTitleRows() {#getPrintTitleRows--}
```
public String getPrintTitleRows()
```


يمثل الصفوف التي تحتوي على الخلايا التي ستُعاد في أعلى كل صفحة.

**Example**

```
         pageSetup.setPrintTitleRows("$1:$1");
```

**Returns:**
java.lang.String
### getPrinterSettings() {#getPrinterSettings--}
```
public byte[] getPrinterSettings()
```


يحصل على إعدادات الطابعة الافتراضية.

**Returns:**
byte[]
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


يمثل حجم الهامش الأيمن، بوحدة السنتيمترات.

**Returns:**
double
### getRightMarginInch() {#getRightMarginInch--}
```
public double getRightMarginInch()
```


يمثل حجم الهامش الأيمن، بوحدة البوصات.

**Returns:**
double
### getTopMargin() {#getTopMargin--}
```
public double getTopMargin()
```


يمثل حجم الهامش العلوي، بوحدة السنتيمترات.

**Returns:**
double
### getTopMarginInch() {#getTopMarginInch--}
```
public double getTopMarginInch()
```


يمثل حجم الهامش العلوي، بوحدة البوصات.

**Returns:**
double
### getZoom() {#getZoom--}
```
public int getZoom()
```


يمثل عامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFirstPageNumber() {#isAutoFirstPageNumber--}
```
public boolean isAutoFirstPageNumber()
```


يشير إلى ما إذا كان رقم الصفحة الأول يتم تعيينه تلقائيًا.

**Returns:**
boolean
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```
public boolean isAutomaticPaperSize()
```


يشير إلى ما إذا كان حجم الورق تلقائيًا.

**Returns:**
boolean
### isHFAlignMargins() {#isHFAlignMargins--}
```
public boolean isHFAlignMargins()
```


يشير إلى ما إذا كانت هوامش الترويسة والتذييل محاذاة مع هوامش الصفحة. إذا كانت هذه الخاصية صحيحة، فسيتم محاذاة الترويسة والتذييل اليساريين مع الهامش الأيسر، والترويسة والتذييل اليمينيين مع الهامش الأيمن. يتم تمكين هذا الخيار افتراضيًا.

**Returns:**
boolean
### isHFDiffFirst() {#isHFDiffFirst--}
```
public boolean isHFDiffFirst()
```


صحيح يعني أن رأس/تذييل الصفحة الأولى مختلف عن الصفحات الأخرى.

**Returns:**
boolean
### isHFDiffOddEven() {#isHFDiffOddEven--}
```
public boolean isHFDiffOddEven()
```


صحيح يعني أن رأس/تذييل الصفحات الفردية مختلف عن الصفحات الفردية.

**Returns:**
boolean
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```
public boolean isHFScaleWithDoc()
```


يشير إلى ما إذا كانت الترويسة والتذييل يتم تحجيمهما مع تحجيم المستند. ينطبق فقط على Excel 2007.

**Returns:**
boolean
### isPercentScale() {#isPercentScale--}
```
public boolean isPercentScale()
```


إذا كانت هذه الخاصية خاطئة، فإن خاصيتي FitToPagesWide وFitToPagesTall تتحكمان في كيفية تحجيم ورقة العمل.

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




### setAutoFirstPageNumber(boolean value) {#setAutoFirstPageNumber-boolean-}
```
public void setAutoFirstPageNumber(boolean value)
```


يشير إلى ما إذا كان رقم الصفحة الأول يتم تعيينه تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBlackAndWhite(boolean value) {#setBlackAndWhite-boolean-}
```
public void setBlackAndWhite(boolean value)
```


يمثل ما إذا كانت عناصر المستند ستُطبع بالأبيض والأسود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBottomMargin(double value) {#setBottomMargin-double-}
```
public void setBottomMargin(double value)
```


يمثل حجم الهامش السفلي، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setBottomMarginInch(double value) {#setBottomMarginInch-double-}
```
public void setBottomMarginInch(double value)
```


يمثل حجم الهامش السفلي، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setCenterHorizontally(boolean value) {#setCenterHorizontally-boolean-}
```
public void setCenterHorizontally(boolean value)
```


يمثل ما إذا كانت الورقة تُطبع متمركزة أفقياً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCenterVertically(boolean value) {#setCenterVertically-boolean-}
```
public void setCenterVertically(boolean value)
```


يمثل ما إذا كانت الورقة تُطبع متمركزة عمودياً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEvenFooter(int section, String footerScript) {#setEvenFooter-int-java.lang.String-}
```
public void setEvenFooter(int section, String footerScript)
```


يضبط سكريبت لتنسيق تذييل الصفحات الزوجية في ملف Excel. يكون له تأثير فقط في Excel 2007 عندما يكون IsHFDiffOddEven صحيحًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| footerScript | java.lang.String | سكريبت تنسيق التذييل. |

### setEvenHeader(int section, String headerScript) {#setEvenHeader-int-java.lang.String-}
```
public void setEvenHeader(int section, String headerScript)
```


يضبط سكريبت لتنسيق ترويسة الصفحات الزوجية في ملف Excel. يكون له تأثير فقط في Excel 2007 عندما يكون IsHFDiffOddEven صحيحًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| headerScript | java.lang.String | سكريبت تنسيق الترويسة. |

### setFirstPageFooter(int section, String footerScript) {#setFirstPageFooter-int-java.lang.String-}
```
public void setFirstPageFooter(int section, String footerScript)
```


يضبط برنامجًا نصيًا لتنسيق تذييل الصفحة الأولى في ملف Excel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| footerScript | java.lang.String | سكريبت تنسيق التذييل. |

### setFirstPageHeader(int section, String headerScript) {#setFirstPageHeader-int-java.lang.String-}
```
public void setFirstPageHeader(int section, String headerScript)
```


يضبط سكريبت لتنسيق ترويسة الصفحة الأولى في ملف Excel. يكون له تأثير فقط في Excel 2007 عندما يكون IsHFDiffFirst صحيحًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| headerScript | java.lang.String | سكريبت تنسيق الترويسة. |

### setFirstPageNumber(int value) {#setFirstPageNumber-int-}
```
public void setFirstPageNumber(int value)
```


يمثل رقم الصفحة الأولى الذي سيُستخدم عند طباعة هذه الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFitToPages(int wide, int tall) {#setFitToPages-int-int-}
```
public void setFitToPages(int wide, int tall)
```


يضبط عدد الصفحات التي سيتم تحجيم ورقة العمل إليها عند طباعتها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| wide | int | صفحات بالعرض. |
| tall | int | صفحات بالطول. |

### setFitToPagesTall(int value) {#setFitToPagesTall-int-}
```
public void setFitToPagesTall(int value)
```


يمثل عدد الصفحات في الارتفاع التي سيتم تحجيم ورقة العمل إليها عند طباعتها. القيمة الافتراضية هي 1.

**Remarks**

يجب ضبط FitToPagesWide على الصفر إذا أردت ملاءمة جميع الصفوف في صفحة واحدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFitToPagesWide(int value) {#setFitToPagesWide-int-}
```
public void setFitToPagesWide(int value)
```


يمثل عدد الصفحات في العرض التي سيتم تحجيم ورقة العمل إليها عند طباعتها. القيمة الافتراضية هي 1.

**Remarks**

يجب ضبط FitToPagesTall على الصفر إذا أردت ملاءمة جميع الأعمدة في صفحة واحدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFooter(int section, String footerScript) {#setFooter-int-java.lang.String-}
```
public void setFooter(int section, String footerScript)
```


يضبط سكريبت لتنسيق تذييل ملف Excel.

**Remarks**

أوامر السكريبت:

| الأمر | الوصف |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | رقم الصفحة الحالي\\u9286\\u20ac |
| &N | عدد الصفحات\\u9286\\u20ac |
| &D | التاريخ الحالي\\u9286\\u20ac |
| &T | الوقت الحالي |
| &A | اسم الورقة |
| &F | اسم الملف بدون المسار |
| &\"<FontName>\" | اسم الخط، على سبيل المثال: &\"Arial\" |
| &\"<FontName>, <FontStyle>\" | اسم الخط ونمط الخط، على سبيل المثال: &\"Arial,Bold\" |
| &<FontSize> | حجم الخط. إذا كان هذا الأمر يليه رقم عادي يُطبع في الترويسة، فسيتم فصله عن ارتفاع الخط بمسافة. |
| &K<RRGGBB> | لون الخط، على سبيل المثال (أحمر): &KFF0000 |
| &G | نص الصورة |

على سبيل المثال: \"&Arial,Bold&8Footer Note\"

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| footerScript | java.lang.String | سكريبت تنسيق التذييل. |

### setFooterMargin(double value) {#setFooterMargin-double-}
```
public void setFooterMargin(double value)
```


يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setFooterMarginInch(double value) {#setFooterMarginInch-double-}
```
public void setFooterMarginInch(double value)
```


يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setFooterPicture(int section, byte[] footerPicture) {#setFooterPicture-int-byte---}
```
public Picture setFooterPicture(int section, byte[] footerPicture)
```


يضبط صورة في تذييل ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| footerPicture | byte[] | بيانات الصورة. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setHFAlignMargins(boolean value) {#setHFAlignMargins-boolean-}
```
public void setHFAlignMargins(boolean value)
```


يشير إلى ما إذا كانت هوامش الترويسة والتذييل محاذاة مع هوامش الصفحة. إذا كانت هذه الخاصية صحيحة، فسيتم محاذاة الترويسة والتذييل اليساريين مع الهامش الأيسر، والترويسة والتذييل اليمينيين مع الهامش الأيمن. يتم تمكين هذا الخيار افتراضيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHFDiffFirst(boolean value) {#setHFDiffFirst-boolean-}
```
public void setHFDiffFirst(boolean value)
```


صحيح يعني أن رأس/تذييل الصفحة الأولى مختلف عن الصفحات الأخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHFDiffOddEven(boolean value) {#setHFDiffOddEven-boolean-}
```
public void setHFDiffOddEven(boolean value)
```


صحيح يعني أن رأس/تذييل الصفحات الفردية مختلف عن الصفحات الفردية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHFScaleWithDoc(boolean value) {#setHFScaleWithDoc-boolean-}
```
public void setHFScaleWithDoc(boolean value)
```


يشير إلى ما إذا كانت الترويسة والتذييل يتم تحجيمهما مع تحجيم المستند. ينطبق فقط على Excel 2007.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHeader(int section, String headerScript) {#setHeader-int-java.lang.String-}
```
public void setHeader(int section, String headerScript)
```


يضبط سكريبت لتنسيق رأس ملف Excel.

**Remarks**

أوامر السكريبت:

| الأمر | الوصف |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | رقم الصفحة الحالي\\u9286\\u20ac |
| &N | عدد الصفحات\\u9286\\u20ac |
| &D | التاريخ الحالي\\u9286\\u20ac |
| &T | الوقت الحالي |
| &A | اسم الورقة |
| &F | اسم الملف بدون المسار |
| &\"<FontName>\" | اسم الخط، على سبيل المثال: &\"Arial\" |
| &\"<FontName>, <FontStyle>\" | اسم الخط ونمط الخط، على سبيل المثال: &\"Arial,Bold\" |
| &<FontSize> | حجم الخط. إذا كان هذا الأمر يليه رقم عادي يُطبع في الترويسة، فسيتم فصله عن ارتفاع الخط بمسافة. |
| &K<RRGGBB> | لون الخط، على سبيل المثال (أحمر): &KFF0000 |
| &G | نص الصورة |

على سبيل المثال: \"&Arial,Bold&8Header Note\"

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| headerScript | java.lang.String | سكريبت تنسيق الترويسة. |

### setHeaderMargin(double value) {#setHeaderMargin-double-}
```
public void setHeaderMargin(double value)
```


يمثل المسافة من أعلى الصفحة إلى الرأس، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHeaderMarginInch(double value) {#setHeaderMarginInch-double-}
```
public void setHeaderMarginInch(double value)
```


يمثل المسافة من أعلى الصفحة إلى الرأس، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHeaderPicture(int section, byte[] headerPicture) {#setHeaderPicture-int-byte---}
```
public Picture setHeaderPicture(int section, byte[] headerPicture)
```


يضبط صورة في رأس ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| headerPicture | byte[] | بيانات الصورة. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


يمثل حجم الهامش الأيسر، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLeftMarginInch(double value) {#setLeftMarginInch-double-}
```
public void setLeftMarginInch(double value)
```


يمثل حجم الهامش الأيسر، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


يمثل الترتيب الذي يستخدمه Microsoft Excel لترقيم الصفحات عند طباعة ورقة عمل كبيرة.

انظر إلى [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


يمثل اتجاه طباعة الصفحة.

انظر [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


يمثل حجم الورق.

انظر [PaperSizeType](../../com.aspose.cells/papersizetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPercentScale(boolean value) {#setPercentScale-boolean-}
```
public void setPercentScale(boolean value)
```


إذا كانت هذه الخاصية خاطئة، فإن خاصيتي FitToPagesWide وFitToPagesTall تتحكمان في كيفية تحجيم ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData) {#setPicture-boolean-boolean-boolean-int-byte---}
```
public Picture setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)
```


يضبط صورة في رأس/تذييل ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isFirst | boolean | يشير إلى ما إذا كان يتم تعيين صورة رأس/تذييل الصفحة الأولى. |
| isEven | boolean | يشير إلى ما إذا كان يتم تعيين صورة رأس/تذييل الصفحات الزوجية. |
| isHeader | boolean | يشير إلى ما إذا كان يتم تعيين صورة رأس/تذييل. |
| القسم | int | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| imageData | byte[] | بيانات الصورة. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setPrintArea(String value) {#setPrintArea-java.lang.String-}
```
public void setPrintArea(String value)
```


يمثل النطاق الذي سيُطبع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPrintComments(int value) {#setPrintComments-int-}
```
public void setPrintComments(int value)
```


يمثل طريقة طباعة التعليقات مع الورقة.

انظر [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPrintCopies(int value) {#setPrintCopies-int-}
```
public void setPrintCopies(int value)
```


يضبط عدد النسخ للطباعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPrintDraft(boolean value) {#setPrintDraft-boolean-}
```
public void setPrintDraft(boolean value)
```


يمثل ما إذا كان سيتم طباعة الورقة بدون رسومات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPrintErrors(int value) {#setPrintErrors-int-}
```
public void setPrintErrors(int value)
```


يحدد نوع خطأ الطباعة المعروض.

انظر إلى [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPrintGridlines(boolean value) {#setPrintGridlines-boolean-}
```
public void setPrintGridlines(boolean value)
```


يمثل ما إذا كانت خطوط الشبكة الخلوية مطبوعة على الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPrintHeadings(boolean value) {#setPrintHeadings-boolean-}
```
public void setPrintHeadings(boolean value)
```


يمثل ما إذا كانت عناوين الصفوف والأعمدة مطبوعة مع هذه الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPrintQuality(int value) {#setPrintQuality-int-}
```
public void setPrintQuality(int value)
```


يمثل جودة الطباعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPrintTitleColumns(String value) {#setPrintTitleColumns-java.lang.String-}
```
public void setPrintTitleColumns(String value)
```


يمثل الأعمدة التي تحتوي على الخلايا التي ستُعاد على الجانب الأيسر من كل صفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPrintTitleRows(String value) {#setPrintTitleRows-java.lang.String-}
```
public void setPrintTitleRows(String value)
```


يمثل الصفوف التي تحتوي على الخلايا التي ستُعاد في أعلى كل صفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPrinterSettings(byte[] value) {#setPrinterSettings-byte---}
```
public void setPrinterSettings(byte[] value)
```


يضبط إعدادات الطابعة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


يمثل حجم الهامش الأيمن، بوحدة السنتيمترات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setRightMarginInch(double value) {#setRightMarginInch-double-}
```
public void setRightMarginInch(double value)
```


يمثل حجم الهامش الأيمن، بوحدة البوصات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTopMargin(double value) {#setTopMargin-double-}
```
public void setTopMargin(double value)
```


يمثل حجم الهامش العلوي، بوحدة السنتيمترات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTopMarginInch(double value) {#setTopMarginInch-double-}
```
public void setTopMarginInch(double value)
```


يمثل حجم الهامش العلوي، بوحدة البوصات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


يمثل عامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

