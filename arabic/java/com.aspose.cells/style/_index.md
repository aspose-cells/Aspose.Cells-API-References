---
title: "Style"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل نمط العرض لمستند إكسل مثل الخط واللون والمحاذاة والحدود إلخ."
type: docs
url: /ar/java/com.aspose.cells/style/
---

**Inheritance:**
java.lang.Object
```
public class Style
```

يمثل نمط العرض لمستند إكسل، مثل الخط واللون والمحاذاة والحدود، إلخ. يحتوي كائن Style على جميع سمات النمط (الخط، تنسيق الأرقام، المحاذاة، وما إلى ذلك) كخصائص.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
         Cell cell = sheets.get(0).getCells().get("A1");
         Style style =  cell.getStyle();
         style.getFont().setName("Times New Roman");
         style.getFont().setColor(Color.getBlue());
         cell.setStyle(style);
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Style()](#Style--) | يُنشئ نسخة جديدة من الفئة [Style](../../com.aspose.cells/style) class. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [copy(Style style)](#copy-com.aspose.cells.Style-) | ينسخ البيانات من كائن نمط آخر |
| [equals(Object obj)](#equals-java.lang.Object-) | يحدد ما إذا كان كائني Style متساويين. |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--) | يحصل على لون الخلفية بقيمة ARGB 32‑بت. |
| [getBackgroundColor()](#getBackgroundColor--) | يحصل على لون خلفية النمط. |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--) | يحصل على لون سمة الخلفية. |
| [getBorders()](#getBorders--) | يحصل على [BorderCollection](../../com.aspose.cells/bordercollection) الخاص بالنمط. |
| [getBottomBorder()](#getBottomBorder--) | يحصل على الحد السفلي. |
| [getClass()](#getClass--) |  |
| [getCultureCustom()](#getCultureCustom--) | يحصل على سلسلة النمط المعتمدة على الثقافة لتنسيق الأرقام. |
| [getCustom()](#getCustom--) | يمثل سلسلة تنسيق الأرقام المخصصة لهذا كائن النمط. |
| [getFont()](#getFont--) | يحصل على كائن [getFont()](../../com.aspose.cells/style\#getFont--) object. |
| [getForegroundArgbColor()](#getForegroundArgbColor--) | يحصل على لون المقدمة بقيمة ARGB 32‑بت. |
| [getForegroundColor()](#getForegroundColor--) | يحصل على لون مقدمة النمط. |
| [getForegroundThemeColor()](#getForegroundThemeColor--) | يحصل على لون سمة المقدمة. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | يحصل على نوع محاذاة النص الأفقي في الخلية. |
| [getIndentLevel()](#getIndentLevel--) | يمثل مستوى المسافة البادئة للخلية أو النطاق. |
| [getInvariantCustom()](#getInvariantCustom--) | يحصل على سلسلة النمط المستقلة عن الثقافة لتنسيق الأرقام. |
| [getLeftBorder()](#getLeftBorder--) | يحصل على الحد الأيسر. |
| [getName()](#getName--) | يحصل على اسم النمط. |
| [getNumber()](#getNumber--) | يحصل على تنسيق العرض للأرقام والتواريخ. |
| [getParentStyle()](#getParentStyle--) | يحصل على النمط الأب لهذا النمط. |
| [getPattern()](#getPattern--) | يحصل على نوع نمط خلفية الخلية. |
| [getQuotePrefix()](#getQuotePrefix--) | يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة. |
| [getRightBorder()](#getRightBorder--) | يحصل على الحد الأيمن. |
| [getRotationAngle()](#getRotationAngle--) | يمثل زاوية دوران النص. |
| [getShrinkToFit()](#getShrinkToFit--) | يمثل ما إذا كان النص ينكمش تلقائيًا ليتناسب مع عرض العمود المتاح. |
| [getTextDirection()](#getTextDirection--) | يمثل ترتيب قراءة النص. |
| [getTopBorder()](#getTopBorder--) | يحصل على الحد العلوي. |
| [getTwoColorGradient()](#getTwoColorGradient--) | احصل على إعداد التدرج اللوني ذو اللونين. |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--) | احصل على إعداد التدرج اللوني ذو اللونين. |
| [getVerticalAlignment()](#getVerticalAlignment--) | يحصل على نوع محاذاة النص العمودي في الخلية. |
| [hasBorders()](#hasBorders--) | يتحقق مما إذا تم تعيين حدود للنمط. |
| [hashCode()](#hashCode--) | يعمل كدالة تجزئة لكائن النمط. |
| [isAlignmentApplied()](#isAlignmentApplied--) | أشر إلى ما إذا كان يجب تطبيق تنسيق المحاذاة. |
| [isBorderApplied()](#isBorderApplied--) | أشر إلى ما إذا كان يجب تطبيق تنسيق الحدود. |
| [isCheckBox()](#isCheckBox--) | يشير إلى ما إذا كان نمطًا لصندوق الاختيار. |
| [isDateTime()](#isDateTime--) | يشير إلى ما إذا كان تنسيق الرقم هو تنسيق تاريخ. |
| [isFillApplied()](#isFillApplied--) | أشر إلى ما إذا كان يجب تطبيق تنسيق التعبئة. |
| [isFontApplied()](#isFontApplied--) | أشر إلى ما إذا كان يجب تطبيق تنسيق الخط. |
| [isFormulaHidden()](#isFormulaHidden--) | يمثل ما إذا كانت الصيغة ستُخفى عندما تكون ورقة العمل محمية. |
| [isGradient()](#isGradient--) | يشير إلى ما إذا كان تظليل الخلية نمطًا متدرجًا. |
| [isJustifyDistributed()](#isJustifyDistributed--) | يشير إلى ما إذا كان يجب استخدام محاذاة الخلايا المبررة أو الموزعة في السطر الأخير من النص. |
| [isLocked()](#isLocked--) | يحصل على قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا. |
| [isModified(int modifyFlag)](#isModified-int-) | يتحقق مما إذا كانت الخصائص المحددة للنمط قد تم تعديلها. |
| [isNumberFormatApplied()](#isNumberFormatApplied--) | يشير إلى ما إذا كان يجب تطبيق تنسيق الأرقام. |
| [isPercent()](#isPercent--) | يشير إلى ما إذا كان تنسيق الرقم هو تنسيق النسبة المئوية. |
| [isProtectionApplied()](#isProtectionApplied--) | يشير إلى ما إذا كان يجب تطبيق تنسيق الحماية. |
| [isTextWrapped()](#isTextWrapped--) | يحصل على قيمة تشير إلى ما إذا كان النص داخل الخلية مُلتفًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentApplied(boolean value)](#setAlignmentApplied-boolean-) | أشر إلى ما إذا كان يجب تطبيق تنسيق المحاذاة. |
| [setBackgroundArgbColor(int value)](#setBackgroundArgbColor-int-) | يضبط لون الخلفية باستخدام قيمة ARGB 32-بت. |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | يضبط لون خلفية النمط. |
| [setBackgroundThemeColor(ThemeColor value)](#setBackgroundThemeColor-com.aspose.cells.ThemeColor-) | يضبط لون سمة الخلفية. |
| [setBorder(int borderType, int borderStyle, CellsColor borderColor)](#setBorder-int-int-com.aspose.cells.CellsColor-) | يضبط حدود النمط. |
| [setBorder(int borderType, int borderStyle, Color borderColor)](#setBorder-int-int-com.aspose.cells.Color-) | يضبط حدود النمط. |
| [setBorderApplied(boolean value)](#setBorderApplied-boolean-) | أشر إلى ما إذا كان يجب تطبيق تنسيق الحدود. |
| [setCheckBox(boolean value)](#setCheckBox-boolean-) | يشير إلى ما إذا كان نمطًا لصندوق الاختيار. |
| [setCultureCustom(String value)](#setCultureCustom-java.lang.String-) | يضبط سلسلة النمط المعتمدة على الثقافة لتنسيق الأرقام. |
| [setCustom(String value)](#setCustom-java.lang.String-) | يمثل سلسلة تنسيق الأرقام المخصصة لهذا كائن النمط. |
| [setCustom(String custom, boolean builtinPreference)](#setCustom-java.lang.String-boolean-) | يضبط سلسلة تنسيق الرقم المخصص للخلية. |
| [setFillApplied(boolean value)](#setFillApplied-boolean-) | أشر إلى ما إذا كان يجب تطبيق تنسيق التعبئة. |
| [setFontApplied(boolean value)](#setFontApplied-boolean-) | أشر إلى ما إذا كان يجب تطبيق تنسيق الخط. |
| [setForegroundArgbColor(int value)](#setForegroundArgbColor-int-) | يضبط لون المقدمة باستخدام قيمة ARGB 32-بت. |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | يضبط لون مقدمة النمط. |
| [setForegroundThemeColor(ThemeColor value)](#setForegroundThemeColor-com.aspose.cells.ThemeColor-) | يضبط لون سمة المقدمة. |
| [setFormulaHidden(boolean value)](#setFormulaHidden-boolean-) | يمثل ما إذا كانت الصيغة ستُخفى عندما تكون ورقة العمل محمية. |
| [setGradient(boolean value)](#setGradient-boolean-) | يشير إلى ما إذا كان تظليل الخلية نمطًا متدرجًا. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | يضبط نوع محاذاة النص الأفقية في الخلية. |
| [setIndentLevel(int value)](#setIndentLevel-int-) | يمثل مستوى المسافة البادئة للخلية أو النطاق. |
| [setJustifyDistributed(boolean value)](#setJustifyDistributed-boolean-) | يشير إلى ما إذا كان يجب استخدام محاذاة الخلايا المبررة أو الموزعة في السطر الأخير من النص. |
| [setLocked(boolean value)](#setLocked-boolean-) | يضبط قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم النمط. |
| [setNumber(int value)](#setNumber-int-) | يضبط تنسيق العرض للأرقام والتواريخ. |
| [setNumberFormatApplied(boolean value)](#setNumberFormatApplied-boolean-) | يشير إلى ما إذا كان يجب تطبيق تنسيق الأرقام. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | اضبط حدود المخطط |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | اضبط حدود المخطط |
| [setPattern(int value)](#setPattern-int-) | يضبط نوع نمط خلفية الخلية. |
| [setPatternColor(int pattern, Color color1, Color color2)](#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-) | يضبط لون الخلفية. |
| [setProtectionApplied(boolean value)](#setProtectionApplied-boolean-) | يشير إلى ما إذا كان يجب تطبيق تنسيق الحماية. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | يمثل زاوية دوران النص. |
| [setShrinkToFit(boolean value)](#setShrinkToFit-boolean-) | يمثل ما إذا كان النص ينكمش تلقائيًا ليتناسب مع عرض العمود المتاح. |
| [setTextDirection(int value)](#setTextDirection-int-) | يمثل ترتيب قراءة النص. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | يضبط قيمة تشير إلى ما إذا كان النص داخل الخلية مُلتفًا. |
| [setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | يضبط التعبئة المحددة لتصبح تدرجًا لونيًا من لونين. |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | يحدد نوع محاذاة النص العمودية في الخلية. |
| [toJson()](#toJson--) | تحويل [Style](../../com.aspose.cells/style) إلى بيانات هيكل JSON. |
| [toString()](#toString--) |  |
| [update()](#update--) | تطبيق النمط المسمى على أنماط الخلايا التي تستخدم هذا النمط المسمى. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Style() {#Style--}
```
public Style()
```


يُنشئ نسخة جديدة من الفئة [Style](../../com.aspose.cells/style) class.

**Remarks**

ملاحظة: هذا المُنشئ أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة CellsFactory.CreateStyle(). سيتم إزالة هذه الخاصية بعد 6 أشهر منذ أكتوبر 2016. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### copy(Style style) {#copy-com.aspose.cells.Style-}
```
public void copy(Style style)
```


ينسخ البيانات من كائن نمط آخر

**Remarks**

هذه الطريقة لا تنسخ اسم النمط. إذا كنت ترغب في نسخ الاسم، يرجى استدعاء الشيفرات التالية بعد نسخ النمط: destStyle.Name = style.Name.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | كائن Style المصدر |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يحدد ما إذا كان كائني Style متساويين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | كائن Style للمقارنة مع كائن Style الحالي. |

**Returns:**
منطقي - true إذا كان الكائن المحدد يساوي الكائن الحالي؛ وإلا false.
### getBackgroundArgbColor() {#getBackgroundArgbColor--}
```
public int getBackgroundArgbColor()
```


يحصل على لون الخلفية بقيمة ARGB 32‑بت.

**Returns:**
int
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


يحصل على لون خلفية النمط.

**Remarks**

إذا كنت ترغب في تعيين لون الخلية، يرجى استخدام خاصية Style.ForegroundColor. فقط إذا كان نمط خلية النمط مختلفًا عن لا شيء أو صلب، ستصبح هذه الخاصية سارية.

**Returns:**
[Color](../../com.aspose.cells/color)
### getBackgroundThemeColor() {#getBackgroundThemeColor--}
```
public ThemeColor getBackgroundThemeColor()
```


يحصل على لون سمة الخلفية.

**Remarks**

إذا لم يكن لون الخلفية لونًا من السمة، سيتم إرجاع NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getBorders() {#getBorders--}
```
public BorderCollection getBorders()
```


يحصل على [BorderCollection](../../com.aspose.cells/bordercollection) الخاص بالنمط.

**Returns:**
[BorderCollection](../../com.aspose.cells/bordercollection)
### getBottomBorder() {#getBottomBorder--}
```
public Border getBottomBorder()
```


يحصل على الحد السفلي.

**Returns:**
[Border](../../com.aspose.cells/border)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCultureCustom() {#getCultureCustom--}
```
public String getCultureCustom()
```


يحصل على سلسلة النمط المعتمدة على الثقافة لتنسيق الأرقام. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج.

**Remarks**

بالنسبة لتنسيق الأرقام المدمج، كل من محتوى النمط (مثلًا، أحد تنسيقات التاريخ المدمجة هو \"m/d/y\" لبعض اللغات، ولكن لبعض اللغات الأخرى يصبح \"d/m/y\") ومحدد التنسيق (مثلًا، بعض اللغات تستخدم حرفًا غير 'y' لتمثيل جزء السنة في تنسيق التاريخ) يعتمد على الثقافة؛ بالنسبة للتنسيق المخصص المحدد من قبل المستخدم، يتم تغيير محددات التنسيق فقط وفقًا للثقافة، ولا يتم تعديل الأجزاء الأخرى من نمط التنسيق.

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


يمثل سلسلة تنسيق الرقم المخصص لهذا كائن النمط. إذا لم يتم تعيين تنسيق الرقم المخصص (على سبيل المثال، تنسيق الرقم مدمج)، سيتم إرجاع \"\".

**Remarks**

السلسلة المخصصة المرتجعة غير معتمدة على الثقافة.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


يحصل على كائن [getFont()](../../com.aspose.cells/style\#getFont--) object.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForegroundArgbColor() {#getForegroundArgbColor--}
```
public int getForegroundArgbColor()
```


يحصل على لون المقدمة بقيمة ARGB 32‑بت.

**Returns:**
int
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


يحصل على لون مقدمة النمط.

**Remarks**

يعني عدم تعيين لون إذا تم إرجاع Color.Empty.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForegroundThemeColor() {#getForegroundThemeColor--}
```
public ThemeColor getForegroundThemeColor()
```


يحصل على لون سمة المقدمة.

**Remarks**

إذا لم يكن لون المقدمة لونًا من السمة، سيتم إرجاع NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


يحصل على نوع محاذاة النص الأفقي في الخلية.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


يمثل مستوى المسافة البادئة للخلية أو النطاق. يمكن أن يكون عددًا صحيحًا فقط من 0 إلى 250.

**Remarks**

إذا تم تعيين نوع محاذاة النص الأفقية إلى قيمة غير اليسار أو اليمين، سيتم إعادة تعيين مستوى المسافة البادئة إلى الصفر.

**Returns:**
int
### getInvariantCustom() {#getInvariantCustom--}
```
public String getInvariantCustom()
```


يحصل على سلسلة النمط غير المعتمدة على الثقافة لتنسيق الأرقام. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج.

**Remarks**

بالنسبة لتنسيقات الأرقام المدمجة، لا يزال محتوى النمط المرتجع يعتمد على الثقافة، مثلًا، لبعض اللغات يعيد \"m/d/y\" ولغات أخرى يعيد \"d/m/y\". الفرق عن [getCultureCustom()](../../com.aspose.cells/style\\#getCultureCustom--) هو (وهذا ما يعنيه أيضًا عدم الاعتماد على الثقافة): يتم الحفاظ على محددات التنسيق والفواصل كمعايير، مثل '/' سيُستخدم دائمًا كفاصل تاريخ/وقت و \"y\" سيُستخدم دائمًا كجزء \"السنة\" بغض النظر عن أي حرف خاص آخر يُستخدم للغة المحددة.

**Returns:**
java.lang.String
### getLeftBorder() {#getLeftBorder--}
```
public Border getLeftBorder()
```


يحصل على الحد الأيسر.

**Returns:**
[Border](../../com.aspose.cells/border)
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم النمط.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


يحصل على تنسيق العرض للأرقام والتواريخ. أنماط التنسيق تختلف بين المناطق.

**Remarks**

على سبيل المثال، أنماط التنسيق الممثلة بأرقام لمنطقة en\\_US:

| Value | نوع | سلسلة التنسيق |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[أحمر](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[أحمر](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm ص/م` |
| 19 | Time | `h:mm:ss ص/م` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[أحمر](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[أحمر](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getParentStyle() {#getParentStyle--}
```
public Style getParentStyle()
```


يحصل على النمط الأب لهذا النمط.

**Returns:**
[Style](../../com.aspose.cells/style)
### getPattern() {#getPattern--}
```
public int getPattern()
```


يحصل على نوع نمط خلفية الخلية.

انظر [BackgroundType](../../com.aspose.cells/backgroundtype).

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة.

**Returns:**
boolean
### getRightBorder() {#getRightBorder--}
```
public Border getRightBorder()
```


يحصل على الحد الأيمن.

**Returns:**
[Border](../../com.aspose.cells/border)
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


يمثل زاوية دوران النص.

**Remarks**

0: غير مدور.

255: من الأعلى إلى الأسفل.

\-90: إلى الأسفل.

90: إلى الأعلى.

يمكنك تعيين 255 أو قيمة تتراوح من -90 إلى 90.

**Returns:**
int
### getShrinkToFit() {#getShrinkToFit--}
```
public boolean getShrinkToFit()
```


يمثل ما إذا كان النص ينكمش تلقائيًا ليتناسب مع عرض العمود المتاح.

**Returns:**
boolean
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


يمثل ترتيب قراءة النص.

انظر [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getTopBorder() {#getTopBorder--}
```
public Border getTopBorder()
```


يحصل على الحد العلوي.

**Returns:**
[Border](../../com.aspose.cells/border)
### getTwoColorGradient() {#getTwoColorGradient--}
```
public Object[] getTwoColorGradient()
```


احصل على إعداد التدرج اللوني ذو اللونين.

**Remarks**

ملاحظة: هذه الطريقة أصبحت مهجورة الآن. بدلاً من ذلك، يرجى استخدام طريقة Style.GetTwoColorGradientSetting(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.Object[] - يُرجع جميع الإعدادات المتعلقة بتدرج اللونين [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant
### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}
```
public TwoColorGradient getTwoColorGradientSetting()
```


احصل على إعداد التدرج اللوني ذو اللونين.

**Returns:**
[TwoColorGradient](../../com.aspose.cells/twocolorgradient)
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


يحصل على نوع محاذاة النص العمودي في الخلية.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### hasBorders() {#hasBorders--}
```
public boolean hasBorders()
```


يتحقق مما إذا تم تعيين حدود للنمط.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعمل كدالة تجزئة لكائن النمط.

**Remarks**

هذه الطريقة مخصصة للاستخدام الداخلي فقط.

**Returns:**
int - رمز تجزئة (hash code) للكائن الحالي.
### isAlignmentApplied() {#isAlignmentApplied--}
```
public boolean isAlignmentApplied()
```


أشر إلى ما إذا كان يجب تطبيق تنسيق المحاذاة.

**Remarks**

فقط للنمط المسمى.

**Returns:**
boolean
### isBorderApplied() {#isBorderApplied--}
```
public boolean isBorderApplied()
```


أشر إلى ما إذا كان يجب تطبيق تنسيق الحدود.

**Remarks**

فقط للنمط المسمى.

**Returns:**
boolean
### isCheckBox() {#isCheckBox--}
```
public boolean isCheckBox()
```


يشير إلى ما إذا كان نمطًا لصندوق الاختيار.

**Returns:**
boolean
### isDateTime() {#isDateTime--}
```
public boolean isDateTime()
```


يشير إلى ما إذا كان تنسيق الرقم هو تنسيق تاريخ.

**Returns:**
boolean
### isFillApplied() {#isFillApplied--}
```
public boolean isFillApplied()
```


أشر إلى ما إذا كان يجب تطبيق تنسيق التعبئة.

**Remarks**

فقط للنمط المسمى.

**Returns:**
boolean
### isFontApplied() {#isFontApplied--}
```
public boolean isFontApplied()
```


أشر إلى ما إذا كان يجب تطبيق تنسيق الخط.

**Remarks**

فقط للنمط المسمى.

**Returns:**
boolean
### isFormulaHidden() {#isFormulaHidden--}
```
public boolean isFormulaHidden()
```


يمثل ما إذا كانت الصيغة ستُخفى عندما تكون ورقة العمل محمية.

**Returns:**
boolean
### isGradient() {#isGradient--}
```
public boolean isGradient()
```


يشير إلى ما إذا كان تظليل الخلية نمطًا متدرجًا.

**Returns:**
boolean
### isJustifyDistributed() {#isJustifyDistributed--}
```
public boolean isJustifyDistributed()
```


يشير إلى ما إذا كان يجب استخدام محاذاة الخلايا المبررة أو الموزعة في السطر الأخير من النص.

**Remarks**

هذا شائع لتنسيقات شرق آسيا لكنه غير شائع في السياقات الأخرى. يعمل فقط عندما تكون المحاذاة الأفقية موزعة.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


يحصل على قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا.

**Remarks**

قفل الخلايا لا يؤثر إلا إذا كانت ورقة العمل محمية.

**Returns:**
boolean
### isModified(int modifyFlag) {#isModified-int-}
```
public boolean isModified(int modifyFlag)
```


يتحقق مما إذا كانت الخصائص المحددة للنمط قد تم تعديلها. يُستخدم لنمط التنسيقات الشرطية للتحقق مما إذا كان يجب استخدام الخصائص المحددة لهذا النمط عند تطبيق التنسيقات الشرطية على خلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| modifyFlag | int | [StyleModifyFlag](../../com.aspose.cells/stylemodifyflag). علامات تعديل النمط |

**Returns:**
boolean - true إذا تم تعديل الخصائص المحددة
### isNumberFormatApplied() {#isNumberFormatApplied--}
```
public boolean isNumberFormatApplied()
```


يشير إلى ما إذا كان يجب تطبيق تنسيق الأرقام.

**Remarks**

فقط للنمط المسمى.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


يشير إلى ما إذا كان تنسيق الرقم هو تنسيق النسبة المئوية.

**Returns:**
boolean
### isProtectionApplied() {#isProtectionApplied--}
```
public boolean isProtectionApplied()
```


يشير إلى ما إذا كان يجب تطبيق تنسيق الحماية.

**Remarks**

فقط للنمط المسمى.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


يحصل على قيمة تشير إلى ما إذا كان النص داخل الخلية مُلتفًا.

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




### setAlignmentApplied(boolean value) {#setAlignmentApplied-boolean-}
```
public void setAlignmentApplied(boolean value)
```


أشر إلى ما إذا كان يجب تطبيق تنسيق المحاذاة.

**Remarks**

فقط للنمط المسمى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBackgroundArgbColor(int value) {#setBackgroundArgbColor-int-}
```
public void setBackgroundArgbColor(int value)
```


يضبط لون الخلفية باستخدام قيمة ARGB 32-بت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


يضبط لون خلفية النمط.

**Remarks**

إذا كنت ترغب في تعيين لون الخلية، يرجى استخدام خاصية Style.ForegroundColor. فقط إذا كان نمط خلية النمط مختلفًا عن لا شيء أو صلب، ستصبح هذه الخاصية سارية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBackgroundThemeColor(ThemeColor value) {#setBackgroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setBackgroundThemeColor(ThemeColor value)
```


يضبط لون سمة الخلفية.

**Remarks**

إذا لم يكن لون الخلفية لونًا من السمة، سيتم إرجاع NULL.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setBorder(int borderType, int borderStyle, CellsColor borderColor) {#setBorder-int-int-com.aspose.cells.CellsColor-}
```
public boolean setBorder(int borderType, int borderStyle, CellsColor borderColor)
```


يضبط حدود النمط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). الحدود التي سيتم تعيينها، يمكن أن تكون مزيجًا من [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نمط الحد. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | لون الحد. |

**Returns:**
boolean - ما إذا تم تغيير إعدادات الحد الحالية.
### setBorder(int borderType, int borderStyle, Color borderColor) {#setBorder-int-int-com.aspose.cells.Color-}
```
public boolean setBorder(int borderType, int borderStyle, Color borderColor)
```


يضبط حدود النمط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). الحدود التي سيتم تعيينها، يمكن أن تكون مزيجًا من [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نمط الحد. |
| borderColor | [Color](../../com.aspose.cells/color) | لون الحد. |

**Returns:**
boolean - ما إذا تم تغيير إعدادات الحد الحالية.
### setBorderApplied(boolean value) {#setBorderApplied-boolean-}
```
public void setBorderApplied(boolean value)
```


أشر إلى ما إذا كان يجب تطبيق تنسيق الحدود.

**Remarks**

فقط للنمط المسمى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckBox(boolean value) {#setCheckBox-boolean-}
```
public void setCheckBox(boolean value)
```


يشير إلى ما إذا كان نمطًا لصندوق الاختيار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCultureCustom(String value) {#setCultureCustom-java.lang.String-}
```
public void setCultureCustom(String value)
```


يضبط سلسلة النمط المعتمدة على الثقافة لتنسيق الأرقام. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج.

**Remarks**

بالنسبة لتنسيق الأرقام المدمج، كل من محتوى النمط (مثلًا، أحد تنسيقات التاريخ المدمجة هو \"m/d/y\" لبعض اللغات، ولكن لبعض اللغات الأخرى يصبح \"d/m/y\") ومحدد التنسيق (مثلًا، بعض اللغات تستخدم حرفًا غير 'y' لتمثيل جزء السنة في تنسيق التاريخ) يعتمد على الثقافة؛ بالنسبة للتنسيق المخصص المحدد من قبل المستخدم، يتم تغيير محددات التنسيق فقط وفقًا للثقافة، ولا يتم تعديل الأجزاء الأخرى من نمط التنسيق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


يمثل سلسلة تنسيق الرقم المخصص لهذا كائن النمط. إذا لم يتم تعيين تنسيق الرقم المخصص (على سبيل المثال، تنسيق الرقم مدمج)، سيتم إرجاع \"\".

**Remarks**

السلسلة المخصصة المرتجعة غير معتمدة على الثقافة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCustom(String custom, boolean builtinPreference) {#setCustom-java.lang.String-boolean-}
```
public void setCustom(String custom, boolean builtinPreference)
```


يضبط سلسلة تنسيق الرقم المخصص للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مخصص | java.lang.String | سلسلة تنسيق الرقم المخصص، يجب أن تكون بنمط InvariantCulture. |
| builtinPreference | boolean | إذا كانت سلسلة تنسيق الرقم المخصص المطابقة تتطابق مع أحد تنسيقات الأرقام المدمجة المقابلة لإعدادات المنطقة الحالية، فهل يتم تعيين تنسيق الرقم كمدمج بدلاً من مخصص. |

### setFillApplied(boolean value) {#setFillApplied-boolean-}
```
public void setFillApplied(boolean value)
```


أشر إلى ما إذا كان يجب تطبيق تنسيق التعبئة.

**Remarks**

فقط للنمط المسمى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFontApplied(boolean value) {#setFontApplied-boolean-}
```
public void setFontApplied(boolean value)
```


أشر إلى ما إذا كان يجب تطبيق تنسيق الخط.

**Remarks**

فقط للنمط المسمى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setForegroundArgbColor(int value) {#setForegroundArgbColor-int-}
```
public void setForegroundArgbColor(int value)
```


يضبط لون المقدمة باستخدام قيمة ARGB 32-بت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


يضبط لون مقدمة النمط.

**Remarks**

يعني عدم تعيين لون إذا تم إرجاع Color.Empty.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundThemeColor(ThemeColor value) {#setForegroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setForegroundThemeColor(ThemeColor value)
```


يضبط لون سمة المقدمة.

**Remarks**

إذا لم يكن لون المقدمة لونًا من السمة، سيتم إرجاع NULL.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setFormulaHidden(boolean value) {#setFormulaHidden-boolean-}
```
public void setFormulaHidden(boolean value)
```


يمثل ما إذا كانت الصيغة ستُخفى عندما تكون ورقة العمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setGradient(boolean value) {#setGradient-boolean-}
```
public void setGradient(boolean value)
```


يشير إلى ما إذا كان تظليل الخلية نمطًا متدرجًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


يضبط نوع محاذاة النص الأفقية في الخلية.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


يمثل مستوى المسافة البادئة للخلية أو النطاق. يمكن أن يكون عددًا صحيحًا فقط من 0 إلى 250.

**Remarks**

إذا تم تعيين نوع محاذاة النص الأفقية إلى قيمة غير اليسار أو اليمين، سيتم إعادة تعيين مستوى المسافة البادئة إلى الصفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setJustifyDistributed(boolean value) {#setJustifyDistributed-boolean-}
```
public void setJustifyDistributed(boolean value)
```


يشير إلى ما إذا كان يجب استخدام محاذاة الخلايا المبررة أو الموزعة في السطر الأخير من النص.

**Remarks**

هذا شائع لتنسيقات شرق آسيا لكنه غير شائع في السياقات الأخرى. يعمل فقط عندما تكون المحاذاة الأفقية موزعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا.

**Remarks**

قفل الخلايا لا يؤثر إلا إذا كانت ورقة العمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم النمط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


يضبط تنسيق عرض الأرقام والتواريخ. أنماط التنسيق تختلف بين المناطق.

**Remarks**

على سبيل المثال، أنماط التنسيق الممثلة بأرقام لمنطقة en\\_US:

| Value | نوع | سلسلة التنسيق |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[أحمر](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[أحمر](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm ص/م` |
| 19 | Time | `h:mm:ss ص/م` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[أحمر](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[أحمر](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setNumberFormatApplied(boolean value) {#setNumberFormatApplied-boolean-}
```
public void setNumberFormatApplied(boolean value)
```


يشير إلى ما إذا كان يجب تطبيق تنسيق الأرقام.

**Remarks**

فقط للنمط المسمى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


اضبط حدود المخطط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نوع الحدود. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | لون الحدود |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


اضبط حدود المخطط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نوع الحدود. |
| borderColor | [Color](../../com.aspose.cells/color) | لون الحدود |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


يضبط نوع نمط خلفية الخلية.

انظر [BackgroundType](../../com.aspose.cells/backgroundtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPatternColor(int pattern, Color color1, Color color2) {#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-}
```
public void setPatternColor(int pattern, Color color1, Color color2)
```


يضبط لون الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). النمط. |
| color1 | [Color](../../com.aspose.cells/color) | لون المقدمة. |
| color2 | [Color](../../com.aspose.cells/color) | لون الخلفية. يعمل فقط عندما لا يكون النمط هو BackgroundType.None وBackgroundType.Solid. |

### setProtectionApplied(boolean value) {#setProtectionApplied-boolean-}
```
public void setProtectionApplied(boolean value)
```


يشير إلى ما إذا كان يجب تطبيق تنسيق الحماية.

**Remarks**

فقط للنمط المسمى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


يمثل زاوية دوران النص.

**Remarks**

0: غير مدور.

255: من الأعلى إلى الأسفل.

\-90: إلى الأسفل.

90: إلى الأعلى.

يمكنك تعيين 255 أو قيمة تتراوح من -90 إلى 90.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShrinkToFit(boolean value) {#setShrinkToFit-boolean-}
```
public void setShrinkToFit(boolean value)
```


يمثل ما إذا كان النص ينكمش تلقائيًا ليتناسب مع عرض العمود المتاح.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


يمثل ترتيب قراءة النص.

انظر [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان النص داخل الخلية مُلتفًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)
```


يضبط التعبئة المحددة لتصبح تدرجًا لونيًا من لونين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | لون تدرج واحد. |
| color2 | [Color](../../com.aspose.cells/color) | لونان متدرجان. |
| gradientStyleType | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). نمط تظليل التدرج. |
| متغيّر | int | متغيّر التدرج. يمكن أن تكون قيمة من 1 إلى 4، تتطابق مع أحد المتغيّرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان النمط هو GradientStyle.FromCenter، لا يمكن أن يكون معامل Variant سوى 1 أو 2. |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


يحدد نوع محاذاة النص العمودية في الخلية.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### toJson() {#toJson--}
```
public String toJson()
```


تحويل [Style](../../com.aspose.cells/style) إلى بيانات هيكل JSON.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### update() {#update--}
```
public void update()
```


تطبيق النمط المسمى على أنماط الخلايا التي تستخدم هذا النمط المسمى. يعمل كما لو تم النقر على زر "ok" بعد الانتهاء من تعديل النمط. يطبق فقط على النمط المسمى.

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

