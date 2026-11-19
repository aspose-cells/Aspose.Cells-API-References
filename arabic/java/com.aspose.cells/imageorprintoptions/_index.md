---
title: "ImageOrPrintOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يسمح بتحديد الخيارات عند تحويل ورقة العمل إلى صور أو طباعة ورقة العمل أو تحويل المخطط إلى صورة."
type: docs
url: /ar/java/com.aspose.cells/imageorprintoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImageOrPrintOptions
```

يسمح بتحديد الخيارات عند تحويل ورقة العمل إلى صور، أو طباعة ورقة العمل، أو تحويل المخطط إلى صورة.

**Example**

```
         //Set Image Or Print Options
         ImageOrPrintOptions options = new ImageOrPrintOptions();
 
         //Set output image format
         options.setImageType(ImageType.PNG);
 
         //Set Horizontal resolution
         options.setHorizontalResolution(300);
 
         //Set Vertical Resolution
         options.setVerticalResolution(300);
 
         //Instantiate Workbook
         Workbook book = new Workbook("test.xls");
 
         //Save chart as Image using ImageOrPrint Options
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.png", options);
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ImageOrPrintOptions()](#ImageOrPrintOptions--) | منشئ. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | إذا كان AllColumnsInOnePagePerSheet true، سيتم إخراج محتوى جميع الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. |
| [getChartImageType()](#getChartImageType--) | حدد نوع صورة المخطط عند التحويل. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | عند كون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. |
| [getClass()](#getClass--) |  |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | يحصل على الإعدادات المخصصة أثناء التصيير. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | يحصل على لغة التحرير الافتراضية. |
| [getDefaultFont()](#getDefaultFont--) | عند كون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | يُنفّذ هذه الواجهة للحصول على DrawObject و Bound عند التصيير. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | حدد اسم ملف الصورة المضمنة في svg. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | إعداد لتصيير ملفات Emf الميتا في ملف المصدر. |
| [getGridlineColor()](#getGridlineColor--) | يحصل على لون خط الشبكة. |
| [getGridlineType()](#getGridlineType--) | يحصل على نوع خطوط الشبكة. |
| [getHorizontalResolution()](#getHorizontalResolution--) | يحصل على الدقة الأفقية للصور المُولدة، بوحدة النقاط في البوصة. |
| [getImageType()](#getImageType--) | يحصل على تنسيق الصور المُولدة. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | إذا كان OnePagePerSheet true، سيتم إخراج جميع محتويات ورقة واحدة إلى صفحة واحدة فقط في النتيجة. |
| [getOnlyArea()](#getOnlyArea--) | إذا كانت هذه الخاصية صحيحة، سيتم إخراج منطقة واحدة، ولن يُطبق أي مقياس. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد شيء للطباعة. |
| [getPageCount()](#getPageCount--) | يحصل على عدد الصفحات التي سيتم حفظها. |
| [getPageIndex()](#getPageIndex--) | يحصل على الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها. |
| [getPageSavingCallback()](#getPageSavingCallback--) | التحكم/الإشارة إلى تقدم عملية حفظ الصفحة. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | إذا كان PrintWithStatusDialog = true، سيظهر حوار يعرض حالة الطباعة الحالية. |
| [getPrintingPage()](#getPrintingPage--) | يشير إلى الصفحات التي لن تُطبع. |
| [getQuality()](#getQuality--) | يحصل على قيمة تحدد جودة الصور المُولدة لتُطبق فقط عند حفظ الصفحات بتنسيق `Jpeg`. |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | إذا كانت هذه الخاصية صحيحة، فإن الـ svg المُولد سيتناسب مع منطقة العرض. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على نوع تنسيق ملف الإخراج يدعم Tiff/XPS |
| [getSheetSet()](#getSheetSet--) | يحصل على الأوراق التي سيتم عرضها. |
| [getSvgCssPrefix()](#getSvgCssPrefix--) | يحصل على بادئة اسم الـ css في svg، القيمة الافتراضية هي سلسلة فارغة. |
| [getTextCrossType()](#getTextCrossType--) | يحصل على نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية. |
| [getTiffColorDepth()](#getTiffColorDepth--) | يحصل على عمق البت لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`. |
| [getTiffCompression()](#getTiffCompression--) | يحصل على نوع الضغط لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`. |
| [getTiffPhotometricInterpretation()](#getTiffPhotometricInterpretation--) | يحصل على نوع PhotometricInterpretation لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`. |
| [getTransparent()](#getTransparent--) | يشير إلى ما إذا كان خلفية الصورة المُولدة يجب أن تكون شفافة. |
| [getVerticalResolution()](#getVerticalResolution--) | يحصل على الدقة العمودية للصور المُولدة، بوحدة النقاط في البوصة. |
| [getWarningCallback()](#getWarningCallback--) | يحصل على رد النداء للتحذير. |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | يشير إلى ما إذا كان عرض وارتفاع الخلايا يتم ضبطه تلقائيًا وفقًا لقيمة الخلية. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. |
| [isOptimized()](#isOptimized--) | يشير إلى ما إذا كان يجب تحسين عناصر الإخراج. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | إذا كان AllColumnsInOnePagePerSheet true، سيتم إخراج محتوى جميع الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) | يشير إلى ما إذا كان عرض وارتفاع الخلايا يتم ضبطه تلقائيًا وفقًا لقيمة الخلية. |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) | حدد نوع صورة المخطط عند التحويل. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | عند كون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | يضبط الإعدادات المخصصة أثناء التصيير. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | يضبط لغة التحرير الافتراضية. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | عند كون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | يضبط العرض والارتفاع المطلوبين للصورة. |
| [setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)](#setDesiredSize-int-int-boolean-) | يضبط العرض والارتفاع المطلوبين للصورة. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | يُنفّذ هذه الواجهة للحصول على DrawObject و Bound عند التصيير. |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) | حدد اسم ملف الصورة المضمنة في svg. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | إعداد لتصيير ملفات Emf الميتا في ملف المصدر. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | يضبط لون خطوط الشبكة. |
| [setGridlineType(int value)](#setGridlineType-int-) | يضبط نوع خطوط الشبكة. |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) | يضبط الدقة الأفقية للصور المُنشأة، بوحدة النقاط في البوصة. |
| [setImageType(int value)](#setImageType-int-) | يضبط تنسيق الصور المُنشأة. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | إذا كان OnePagePerSheet true، سيتم إخراج جميع محتويات ورقة واحدة إلى صفحة واحدة فقط في النتيجة. |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) | إذا كانت هذه الخاصية صحيحة، سيتم إخراج منطقة واحدة، ولن يُطبق أي مقياس. |
| [setOptimized(boolean value)](#setOptimized-boolean-) | يشير إلى ما إذا كان يجب تحسين عناصر الإخراج. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد شيء للطباعة. |
| [setPageCount(int value)](#setPageCount-int-) | يضبط عدد الصفحات التي سيتم حفظها. |
| [setPageIndex(int value)](#setPageIndex-int-) | يضبط الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | التحكم/الإشارة إلى تقدم عملية حفظ الصفحة. |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) | إذا كان PrintWithStatusDialog = true، سيظهر حوار يعرض حالة الطباعة الحالية. |
| [setPrintingPage(int value)](#setPrintingPage-int-) | يشير إلى الصفحات التي لن تُطبع. |
| [setQuality(int value)](#setQuality-int-) | يضبط قيمة تحدد جودة الصور المُنشأة لتُطبق فقط عند حفظ الصفحات بتنسيق `Jpeg`. |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | يضبط قيمة تفضيل واحد لخوارزميات العرض. |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) | إذا كانت هذه الخاصية صحيحة، فإن الـ svg المُولد سيتناسب مع منطقة العرض. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | يضبط نوع تنسيق ملف الإخراج يدعم Tiff/XPS |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | يضبط الأوراق التي سيتم عرضها. |
| [setSvgCssPrefix(String value)](#setSvgCssPrefix-java.lang.String-) | يضبط بادئة اسم الـ css في svg، القيمة الافتراضية هي سلسلة فارغة. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | يضبط نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية. |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) | يضبط عمق البت لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | يضبط نوع الضغط لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`. |
| [setTiffPhotometricInterpretation(int value)](#setTiffPhotometricInterpretation-int-) | يضبط نوع PhotometricInterpretation لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | يشير إلى ما إذا كان خلفية الصورة المُولدة يجب أن تكون شفافة. |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) | يضبط الدقة العمودية للصور المُنشأة، بوحدة النقاط في البوصة. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | يضبط رد النداء للتحذير. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImageOrPrintOptions() {#ImageOrPrintOptions--}
```
public ImageOrPrintOptions()
```


منشئ.

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


إذا كان AllColumnsInOnePagePerSheet صحيحًا، فسيتم إخراج محتوى جميع الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون عرض حجم الورق في إعدادات الصفحة غير صالح، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية.

**Returns:**
boolean
### getChartImageType() {#getChartImageType--}
```
public ImageFormat getChartImageType()
```


حدد نوع صورة المخطط عند التحويل. القيمة الافتراضية: PNG.

**Remarks**

NOTE: هذا العضو الآن مهمل. بدلاً من ذلك، يتم دائمًا عرض **Chart** و **Shape** كعناصر متجهية (مثل النقطة، الخط) لتحسين جودة العرض. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر كمربعات في PDF أو صورة. اضبط هذا إلى true لمحاولة استخدام الخط الافتراضي للدفتر لإظهار هذه الأحرف أولاً.

**Remarks**

القيمة الافتراضية هي true.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


يحصل على الإعدادات المخصصة أثناء التصيير.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


يحصل على لغة التحرير الافتراضية.

انظر [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

قد يعرض/يُصوّر تخطيطات مختلفة لفقرة النص عندما يتم تعيين لغات تحرير مختلفة. القيمة الافتراضية هي [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر كمربعات في PDF أو صورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لإظهار هذه الأحرف. إذا لم يتم ضبط هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لإظهار هذه الأحرف اليونيكود.

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


يُنفّذ هذه الواجهة للحصول على DrawObject و Bound عند التصيير.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```


حدد اسم ملف الصورة المضمنة في svg. يجب أن يكون مسارًا كاملاً مع الدليل مثل "c:\\\\xpsEmbedded"

**Remarks**

NOTE: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى إزالة هذه الخاصية لأن الصور الآن دائمًا مضمَّنة في Svg بتنسيق base64. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أبريل 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


إعداد لتصيير ملفات Emf الميتا في ملف المصدر.

انظر [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

ملفات EMF التي تم تحديدها كـ "EMF+ Dual" يمكن أن تحتوي على سجلات EMF+ وسجلات EMF. يمكن استخدام أي نوع من السجلات لعرض الصورة، أو سجلات EMF+ فقط، أو سجلات EMF فقط. عندما يتم تعيين [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER)، سيتم تحليل سجلات EMF+ أثناء العرض إلى الصورة، وإلا سيتم تحليل سجلات EMF فقط. القيمة الافتراضية هي [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). بالنسبة للأطر التي تعتمد على .NET System.Drawing.Common، يتم تجاهل هذا الإعداد.

**Returns:**
int
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


يحصل على لون خط الشبكة.

**Remarks**

سيتجاهل إعدادات لون خطوط الشبكة في ملف المصدر.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


يحصل على نوع خطوط الشبكة.

انظر [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

القيمة الافتراضية هي النوع المنقط.

**Returns:**
int
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```


يحصل على الدقة الأفقية للصور المُولدة، بوحدة النقاط في البوصة.

**Remarks**

القيمة الافتراضية هي 96. يؤثر الضبط  و  على عرض وارتفاع الصورة الناتجة بالبكسل.

**Example**

الكود التالي يضبط الدقة إلى 192، عرض وارتفاع الصورة المُنشأة يصبح ضعف الصورة التي تركت الدقة بقيمتها الافتراضية 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render worksheet page to image.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), opts);
         sr.toImage(0, "Sheet_Page1.png");
```

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


يحصل على تنسيق الصور المُنشأة. القيمة الافتراضية: PNG.

انظر [ImageType](../../com.aspose.cells/imagetype).

**Returns:**
int
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


إذا كان OnePagePerSheet صحيحًا، فسيتم إخراج كل محتوى ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون حجم الورق في pagesetup غير صالح، وستظل الإعدادات الأخرى لـ pagesetup سارية.

**Returns:**
boolean
### getOnlyArea() {#getOnlyArea--}
```
public boolean getOnlyArea()
```


إذا كانت هذه الخاصية صحيحة، سيتم إخراج منطقة واحدة، ولن يُطبق أي مقياس.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد شيء للطباعة.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


يحصل على عدد الصفحات التي سيتم حفظها.

**Remarks**

القيمة الافتراضية هي System.Int32.MaxValue مما يعني أنه سيتم عرض جميع الصفحات.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


يحصل على الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها.

**Remarks**

القيمة الافتراضية هي 0.

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


التحكم/الإشارة إلى تقدم عملية حفظ الصفحة.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}
```
public boolean getPrintWithStatusDialog()
```


إذا كان PrintWithStatusDialog = true، سيظهر حوار يعرض حالة الطباعة الحالية. وإلا لن يظهر أي حوار من هذا النوع.

**Returns:**
boolean
### getPrintingPage() {#getPrintingPage--}
```
public int getPrintingPage()
```


يشير إلى الصفحات التي لن تُطبع.

انظر [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```


يحصل على قيمة تحدد جودة الصور المولدة لتطبيقها فقط عند حفظ الصفحات بتنسيق `Jpeg`. القيمة الافتراضية هي 100

**Remarks**

يؤثر فقط عند الحفظ بصيغة JPEG. يجب أن تكون القيمة بين 0 و 100. القيمة الافتراضية هي 100.

**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```


إذا كانت هذه الخاصية صحيحة، فإن الـ svg المُولد سيتناسب مع منطقة العرض.

**Remarks**

ملاحظة: هذه العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أبريل 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


يحصل على نوع تنسيق ملف الإخراج يدعم Tiff/XPS

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

ملاحظة: هذه العضو الآن غير صالح. بدلاً من ذلك، For Tiff/Svg، استخدم [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); For Xps، استخدم [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) مع [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


يحصل على الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في المصنف: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\\#getVisible--).

**Remarks**

يتم تجاهل الإعداد عندما يُستخدم في [SheetRender](../../com.aspose.cells/sheetrender)

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSvgCssPrefix() {#getSvgCssPrefix--}
```
public String getSvgCssPrefix()
```


يحصل على بادئة اسم الـ css في svg، القيمة الافتراضية هي سلسلة فارغة.

**Remarks**

ملاحظة: هذه العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أبريل 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


يحصل على نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية.

انظر [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```


يحصل على عمق البت لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`.

انظر [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

يؤثر فقط عند الحفظ بصيغة TIFF. إذا تم تعيين TiffCompression إلى CCITT3 أو CCITT4، فلن يؤثر ذلك، وستكون عمق البت للصورة TIFF المولدة دائمًا 1.

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```


يحصل على نوع الضغط لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`.

انظر [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

يؤثر فقط عند الحفظ بصيغة TIFF. القيمة الافتراضية هي Lzw.

**Returns:**
int
### getTiffPhotometricInterpretation() {#getTiffPhotometricInterpretation--}
```
public int getTiffPhotometricInterpretation()
```


يحصل على نوع PhotometricInterpretation لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`.

**Remarks**

يؤثر فقط عند الحفظ بصيغة TIFF. القيمة الافتراضية هي -1، تمثل عدم تطبيق PhotometricInterpretation.

**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```


يشير إلى ما إذا كان خلفية الصورة المُولدة يجب أن تكون شفافة.

**Remarks**

القيمة الافتراضية هي false. وهذا يعني أن خلفية الصور المولدة هي بيضاء.

**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```


يحصل على الدقة العمودية للصور المُولدة، بوحدة النقاط في البوصة.

**Remarks**

القيمة الافتراضية هي 96. يؤثر الضبط  و  على عرض وارتفاع الصورة الناتجة بالبكسل.

**Example**

الكود التالي يضبط الدقة إلى 192، عرض وارتفاع الصورة المُنشأة يصبح ضعف الصورة التي تركت الدقة بقيمتها الافتراضية 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render Chart to image.
         wb.getWorksheets().get(0).getCharts().get(0).toImage("Chart.png", opts);
```

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


يحصل على رد النداء للتحذير.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellAutoFit() {#isCellAutoFit--}
```
public boolean isCellAutoFit()
```


يشير إلى ما إذا كان عرض وارتفاع الخلايا يتم ضبطهما تلقائيًا وفقًا لقيمة الخلية. القيمة الافتراضية هي false.

**Remarks**

ملاحظة: هذه العضو الآن غير صالح. بدلاً من ذلك، هذه الخاصية غير مستخدمة، يرجى إزالة هذه الخاصية.. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه.

**Remarks**

القيمة الافتراضية هي false. سنحاول أولاً الخط الافتراضي لملف Workbook وPdfSaveOption/system لخط الخلية.

**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```


يشير إلى ما إذا كان يجب تحسين عناصر الإخراج.

**Remarks**

القيمة الافتراضية هي false. حاليًا عندما يتم تعيين هذه الخاصية إلى true، سيتم تنفيذ التحسينات التالية: 1. تحسين خطوط الحدود. 2. تحسين حجم الملف أثناء التحويل إلى صورة Svg.

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




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


إذا كان AllColumnsInOnePagePerSheet صحيحًا، فسيتم إخراج محتوى جميع الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون عرض حجم الورق في إعدادات الصفحة غير صالح، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```


يشير إلى ما إذا كان عرض وارتفاع الخلايا يتم ضبطهما تلقائيًا وفقًا لقيمة الخلية. القيمة الافتراضية هي false.

**Remarks**

ملاحظة: هذه العضو الآن غير صالح. بدلاً من ذلك، هذه الخاصية غير مستخدمة، يرجى إزالة هذه الخاصية.. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```


حدد نوع صورة المخطط عند التحويل. القيمة الافتراضية: PNG.

**Remarks**

NOTE: هذا العضو الآن مهمل. بدلاً من ذلك، يتم دائمًا عرض **Chart** و **Shape** كعناصر متجهية (مثل النقطة، الخط) لتحسين جودة العرض. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر كمربعات في PDF أو صورة. اضبط هذا إلى true لمحاولة استخدام الخط الافتراضي للدفتر لإظهار هذه الأحرف أولاً.

**Remarks**

القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


يضبط الإعدادات المخصصة أثناء التصيير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


يضبط لغة التحرير الافتراضية.

انظر [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

قد يعرض/يُصوّر تخطيطات مختلفة لفقرة النص عندما يتم تعيين لغات تحرير مختلفة. القيمة الافتراضية هي [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر كمربعات في PDF أو صورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لإظهار هذه الأحرف. إذا لم يتم ضبط هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لإظهار هذه الأحرف اليونيكود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```


يضبط العرض والارتفاع المطلوبين للصورة.

**Remarks**

ملاحظة: هذه العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام [setDesiredSize(int,int,boolean)](../../com.aspose.cells/imageorprintoptions\#setDesiredSize-int-int-boolean-) عن طريق تعيين المعامل keepAspectRatio إلى false. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| desiredWidth | int | العرض المطلوب بالبكسل |
| desiredHeight | int | الارتفاع المطلوب بالبكسل |

### setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio) {#setDesiredSize-int-int-boolean-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)
```


يضبط العرض والارتفاع المطلوبين للصورة.

**Remarks**

سيكون عرض وارتفاع صورة الإخراج بالبكسل مستندًا فقط إلى العرض والارتفاع المطلوبين المحددين. الـ  و الـ  لن تؤثر على عرض وارتفاع صورة الإخراج في هذه الحالة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| desiredWidth | int | العرض المطلوب بالبكسل |
| desiredHeight | int | الارتفاع المطلوب بالبكسل |
| keepAspectRatio | boolean | ما إذا كان يجب الحفاظ على نسبة العرض إلى الارتفاع للصورة الأصلية |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


يُنفّذ هذه الواجهة للحصول على DrawObject و Bound عند التصيير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```


حدد اسم ملف الصورة المضمنة في svg. يجب أن يكون مسارًا كاملاً مع الدليل مثل "c:\\\\xpsEmbedded"

**Remarks**

NOTE: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى إزالة هذه الخاصية لأن الصور الآن دائمًا مضمَّنة في Svg بتنسيق base64. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أبريل 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


إعداد لتصيير ملفات Emf الميتا في ملف المصدر.

انظر [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

ملفات EMF التي تم تحديدها كـ "EMF+ Dual" يمكن أن تحتوي على سجلات EMF+ وسجلات EMF. يمكن استخدام أي نوع من السجلات لعرض الصورة، أو سجلات EMF+ فقط، أو سجلات EMF فقط. عندما يتم تعيين [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER)، سيتم تحليل سجلات EMF+ أثناء العرض إلى الصورة، وإلا سيتم تحليل سجلات EMF فقط. القيمة الافتراضية هي [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). بالنسبة للأطر التي تعتمد على .NET System.Drawing.Common، يتم تجاهل هذا الإعداد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه.

**Remarks**

القيمة الافتراضية هي false. سنحاول أولاً الخط الافتراضي لملف Workbook وPdfSaveOption/system لخط الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


يضبط لون خطوط الشبكة.

**Remarks**

سيتجاهل إعدادات لون خطوط الشبكة في ملف المصدر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


يضبط نوع خطوط الشبكة.

انظر [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

القيمة الافتراضية هي النوع المنقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```


يضبط الدقة الأفقية للصور المُنشأة، بوحدة النقاط في البوصة.

**Remarks**

القيمة الافتراضية هي 96. يؤثر الضبط  و  على عرض وارتفاع الصورة الناتجة بالبكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```


يحدد تنسيق الصور المولدة. القيمة الافتراضية: PNG.

انظر [ImageType](../../com.aspose.cells/imagetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


إذا كان OnePagePerSheet صحيحًا، فسيتم إخراج كل محتوى ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون حجم الورق في pagesetup غير صالح، وستظل الإعدادات الأخرى لـ pagesetup سارية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```


إذا كانت هذه الخاصية صحيحة، سيتم إخراج منطقة واحدة، ولن يُطبق أي مقياس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```


يشير إلى ما إذا كان يجب تحسين عناصر الإخراج.

**Remarks**

القيمة الافتراضية هي false. حاليًا عندما يتم تعيين هذه الخاصية إلى true، سيتم تنفيذ التحسينات التالية: 1. تحسين خطوط الحدود. 2. تحسين حجم الملف أثناء التحويل إلى صورة Svg.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد شيء للطباعة.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


يضبط عدد الصفحات التي سيتم حفظها.

**Remarks**

القيمة الافتراضية هي System.Int32.MaxValue مما يعني أنه سيتم عرض جميع الصفحات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


يضبط الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها.

**Remarks**

القيمة الافتراضية هي 0.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


التحكم/الإشارة إلى تقدم عملية حفظ الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```


إذا كان PrintWithStatusDialog = true، سيظهر حوار يعرض حالة الطباعة الحالية. وإلا لن يظهر أي حوار من هذا النوع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```


يشير إلى الصفحات التي لن تُطبع.

انظر [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```


يحدد قيمة تحدد جودة الصور المولدة لتطبيقها فقط عند حفظ الصفحات بتنسيق `Jpeg`. القيمة الافتراضية هي 100

**Remarks**

يؤثر فقط عند الحفظ بصيغة JPEG. يجب أن تكون القيمة بين 0 و 100. القيمة الافتراضية هي 100.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRenderingHint(RenderingHints.Key key, Object value) {#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-}
```
public void setRenderingHint(RenderingHints.Key key, Object value)
```


يضبط قيمة تفضيل واحد لخوارزميات العرض. تشمل فئات التلميحات عناصر تحكم لجودة العرض وتوازن الوقت/الجودة العام في عملية العرض. راجع فئة RenderingHints للحصول على تعريفات بعض المفاتيح والقيم الشائعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المفتاح | java.awt.RenderingHints.Key | المفتاح الخاص بالتلميحة التي سيتم ضبطها. |
| القيمة | java.lang.Object | القيمة التي تشير إلى التفضيلات لفئة التلميحة المحددة. |

### setSVGFitToViewPort(boolean value) {#setSVGFitToViewPort-boolean-}
```
public void setSVGFitToViewPort(boolean value)
```


إذا كانت هذه الخاصية صحيحة، فإن الـ svg المُولد سيتناسب مع منطقة العرض.

**Remarks**

ملاحظة: هذه العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أبريل 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


يضبط نوع تنسيق ملف الإخراج يدعم Tiff/XPS

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

ملاحظة: هذه العضو الآن غير صالح. بدلاً من ذلك، For Tiff/Svg، استخدم [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); For Xps، استخدم [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) مع [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


يضبط الأوراق التي سيتم عرضها. القيمة الافتراضية هي جميع الأوراق المرئية في المصنف: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

يتم تجاهل الإعداد عندما يُستخدم في [SheetRender](../../com.aspose.cells/sheetrender)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSvgCssPrefix(String value) {#setSvgCssPrefix-java.lang.String-}
```
public void setSvgCssPrefix(String value)
```


يضبط بادئة اسم الـ css في svg، القيمة الافتراضية هي سلسلة فارغة.

**Remarks**

ملاحظة: هذه العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أبريل 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


يضبط نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية.

انظر [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```


يضبط عمق البت لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`.

انظر [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

يؤثر فقط عند الحفظ بصيغة TIFF. إذا تم تعيين TiffCompression إلى CCITT3 أو CCITT4، فلن يؤثر ذلك، وستكون عمق البت للصورة TIFF المولدة دائمًا 1.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```


يضبط نوع الضغط لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`.

انظر [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

يؤثر فقط عند الحفظ بصيغة TIFF. القيمة الافتراضية هي Lzw.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTiffPhotometricInterpretation(int value) {#setTiffPhotometricInterpretation-int-}
```
public void setTiffPhotometricInterpretation(int value)
```


يضبط نوع PhotometricInterpretation لتُطبق فقط عند حفظ الصفحات بتنسيق `Tiff`.

**Remarks**

يؤثر فقط عند الحفظ بصيغة TIFF. القيمة الافتراضية هي -1، تمثل عدم تطبيق PhotometricInterpretation.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


يشير إلى ما إذا كان خلفية الصورة المُولدة يجب أن تكون شفافة.

**Remarks**

القيمة الافتراضية هي false. وهذا يعني أن خلفية الصور المولدة هي بيضاء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```


يضبط الدقة العمودية للصور المُنشأة، بوحدة النقاط في البوصة.

**Remarks**

القيمة الافتراضية هي 96. يؤثر الضبط  و  على عرض وارتفاع الصورة الناتجة بالبكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


يضبط رد النداء للتحذير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

