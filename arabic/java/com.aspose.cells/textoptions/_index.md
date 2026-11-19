---
title: "TextOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات النص."
type: docs
url: /ar/java/com.aspose.cells/textoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Font](../../com.aspose.cells/font)
```
public class TextOptions extends Font
```

يمثل خيارات النص.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | يتحقق مما إذا كان الخطان متساويين. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | يحصل على اللون بقيمة ARGB 32-بت. |
| [getCapsType()](#getCapsType--) | يحصل على نوع الحروف الكبيرة للنصوص في الشكل. |
| [getCharset()](#getCharset--) | يمثل مجموعة الأحرف. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | يحصل على [Color](../../com.aspose.cells/color) للخط. |
| [getDoubleSize()](#getDoubleSize--) | يحصل على الحجم المزدوج للخط. |
| [getFarEastName()](#getFarEastName--) | يحصل على الاسم FarEast. |
| [getFill()](#getFill--) | يمثل تنسيق التعبئة للنص. |
| [getKerning()](#getKerning--) | يحدد الحد الأدنى لحجم الخط الذي يحدث عنده تقارب الأحرف (kerning) لهذا المقطع النصي. |
| [getLanguageCode()](#getLanguageCode--) | يحصل على لغة واجهة المستخدم. |
| [getLatinName()](#getLatinName--) | يحصل على الاسم اللاتيني. |
| [getName()](#getName--) | يحصل على اسم الشكل. |
| [getOutline()](#getOutline--) | يمثل تنسيق المخطط للنص. |
| [getSchemeType()](#getSchemeType--) | يحصل على نوع المخطط للخط. |
| [getScriptOffset()](#getScriptOffset--) | يحصل على إزاحة النص، بوحدة النسبة المئوية |
| [getShadow()](#getShadow--) | يمثل كائن [ShadowEffect](../../com.aspose.cells/shadoweffect) الذي يحدد تأثير الظل لعنصر المخطط أو الشكل. |
| [getSize()](#getSize--) | يحصل على حجم الخط. |
| [getSpacing()](#getSpacing--) | يحدد التباعد بين الأحرف داخل مقطع نصي. |
| [getStrikeType()](#getStrikeType--) | يحصل على نوع الضربة للنص. |
| [getThemeColor()](#getThemeColor--) | يحصل على لون السمة. |
| [getUnderline()](#getUnderline--) | يحصل على نوع تسطير الخط. |
| [getUnderlineColor()](#getUnderlineColor--) | يحصل على لون التسطير. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | يحصل على قيمة تشير إلى ما إذا كان الخط عريضًا. |
| [isItalic()](#isItalic--) | يحصل على قيمة تشير إلى ما إذا كان الخط مائلًا. |
| [isNormalizeHeights()](#isNormalizeHeights--) | يشير إلى ما إذا كان تطبيع الارتفاع سيُطبق على مقطع النص. |
| [isStrikeout()](#isStrikeout--) | يحصل على قيمة تشير إلى ما إذا كان الخط مشطوبًا مرة واحدة. |
| [isSubscript()](#isSubscript--) | يحصل على قيمة تشير إلى ما إذا كان الخط منخفضًا. |
| [isSuperscript()](#isSuperscript--) | يحصل على قيمة تشير إلى ما إذا كان الخط مرتفعًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | يضبط اللون بقيمة ARGB 32-بت. |
| [setBold(boolean value)](#setBold-boolean-) | يضبط قيمة تشير إلى ما إذا كان الخط عريضًا. |
| [setCapsType(int value)](#setCapsType-int-) | يضبط نوع الحروف الكبيرة للنصوص داخل الشكل. |
| [setCharset(int value)](#setCharset-int-) | يمثل مجموعة الأحرف. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | يضبط الـ[Color](../../com.aspose.cells/color) للخط. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | يضبط الحجم المزدوج للخط. |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | يضبط اسم FarEast. |
| [setItalic(boolean value)](#setItalic-boolean-) | يضبط قيمة تشير إلى ما إذا كان الخط مائلًا. |
| [setKerning(double value)](#setKerning-double-) | يحدد الحد الأدنى لحجم الخط الذي يحدث عنده تقارب الأحرف (kerning) لهذا المقطع النصي. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | يضبط لغة واجهة المستخدم. |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | يضبط الاسم اللاتيني. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم الشكل. |
| [setName(String name, int type)](#setName-java.lang.String-int-) | يضبط الاسم والمخطط للخط. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | يشير إلى ما إذا كان تطبيع الارتفاع سيُطبق على مقطع النص. |
| [setSchemeType(int value)](#setSchemeType-int-) | يضبط نوع المخطط للخط. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | يضبط إزاحة النص، بوحدة النسبة المئوية |
| [setSize(int value)](#setSize-int-) | يضبط حجم الخط. |
| [setSpacing(double value)](#setSpacing-double-) | يحدد التباعد بين الأحرف داخل مقطع نصي. |
| [setStrikeType(int value)](#setStrikeType-int-) | يحصل على نوع الضربة للنص. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | يضبط قيمة تشير إلى ما إذا كان الخط يحتوي على خط مشطوب واحد. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | يضبط قيمة تشير إلى ما إذا كان الخط مكتوبًا كمنخفض. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | يضبط قيمة تشير إلى ما إذا كان الخط مكتوبًا كمرتفع. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | يضبط لون السمة. |
| [setUnderline(int value)](#setUnderline-int-) | يضبط نوع تسطير الخط. |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | يضبط لون التسطير. |
| [toString()](#toString--) | يرجع سلسلة تمثل كائن Cell الحالي. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


يتحقق مما إذا كان الخطان متساويين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | كائن الخط المقارن. |

**Returns:**
منطقي - صحيح إذا كان مساويًا لكائن الخط المقارن.
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


يحصل على اللون بقيمة ARGB 32-بت.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


يحصل على نوع الحروف الكبيرة للنصوص في الشكل.

انظر [TextCapsType](../../com.aspose.cells/textcapstype).

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


يمثل مجموعة الأحرف.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


يحصل على [Color](../../com.aspose.cells/color) للخط.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


يحصل على الحجم المزدوج للخط.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


يحصل على الاسم FarEast.

**Returns:**
java.lang.String
### getFill() {#getFill--}
```
public FillFormat getFill()
```


يمثل تنسيق التعبئة للنص.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getKerning() {#getKerning--}
```
public double getKerning()
```


يحدد الحد الأدنى لحجم الخط الذي يحدث عنده تقارب الأحرف (kerning) لهذا المقطع النصي.

**Returns:**
double
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


يحصل على لغة واجهة المستخدم.

انظر [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


يحصل على الاسم اللاتيني.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم الشكل.

**Returns:**
java.lang.String
### getOutline() {#getOutline--}
```
public LineFormat getOutline()
```


يمثل تنسيق المخطط للنص.

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


يحصل على نوع المخطط للخط.

انظر [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


يحصل على إزاحة النص، بوحدة النسبة المئوية

**Remarks**

فقط للأشكال والرسوم البيانية.

**Returns:**
double
### getShadow() {#getShadow--}
```
public ShadowEffect getShadow()
```


يمثل كائن [ShadowEffect](../../com.aspose.cells/shadoweffect) الذي يحدد تأثير الظل لعنصر المخطط أو الشكل.

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSize() {#getSize--}
```
public int getSize()
```


يحصل على حجم الخط.

**Returns:**
int
### getSpacing() {#getSpacing--}
```
public double getSpacing()
```


يحدد التباعد بين الأحرف داخل مقطع نصي.

**Returns:**
double
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


يحصل على نوع الضربة للنص.

انظر [TextStrikeType](../../com.aspose.cells/textstriketype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


يحصل على لون السمة.

**Remarks**

إذا لم يكن لون الخط لونًا من السمة، سيتم إرجاع NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


يحصل على نوع تسطير الخط.

انظر [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


يحصل على لون التسطير.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBold() {#isBold--}
```
public boolean isBold()
```


يحصل على قيمة تشير إلى ما إذا كان الخط عريضًا.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


يحصل على قيمة تشير إلى ما إذا كان الخط مائلًا.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


يشير إلى ما إذا كان تطبيع الارتفاع سيُطبق على مقطع النص.

**Remarks**

فقط لخطوط الأشكال أو الرسوم البيانية.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


يحصل على قيمة تشير إلى ما إذا كان الخط مشطوبًا مرة واحدة.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


يحصل على قيمة تشير إلى ما إذا كان الخط منخفضًا.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


يحصل على قيمة تشير إلى ما إذا كان الخط مرتفعًا.

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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


يضبط اللون بقيمة ARGB 32-بت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان الخط عريضًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


يضبط نوع الحروف الكبيرة للنصوص داخل الشكل.

انظر [TextCapsType](../../com.aspose.cells/textcapstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


يمثل مجموعة الأحرف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


يضبط الـ[Color](../../com.aspose.cells/color) للخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


يضبط الحجم المزدوج للخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


يضبط اسم FarEast.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان الخط مائلًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


يحدد الحد الأدنى لحجم الخط الذي يحدث عنده تقارب الأحرف (kerning) لهذا المقطع النصي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


يضبط لغة واجهة المستخدم.

انظر [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


يضبط الاسم اللاتيني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


يضبط الاسم والمخطط للخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


يشير إلى ما إذا كان تطبيع الارتفاع سيُطبق على مقطع النص.

**Remarks**

فقط لخطوط الأشكال أو الرسوم البيانية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


يضبط نوع المخطط للخط.

انظر [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


يضبط إزاحة النص، بوحدة النسبة المئوية

**Remarks**

فقط للأشكال والرسوم البيانية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


يضبط حجم الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


يحدد التباعد بين الأحرف داخل مقطع نصي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


يحصل على نوع الضربة للنص.

انظر [TextStrikeType](../../com.aspose.cells/textstriketype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان الخط يحتوي على خط مشطوب واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان الخط مكتوبًا كمنخفض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان الخط مكتوبًا كمرتفع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


يضبط لون السمة.

**Remarks**

إذا لم يكن لون الخط لونًا من السمة، سيتم إرجاع NULL.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


يضبط نوع تسطير الخط.

انظر [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


يضبط لون التسطير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### toString() {#toString--}
```
public String toString()
```


يرجع سلسلة تمثل كائن Cell الحالي.

**Returns:**
java.lang.String -
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

