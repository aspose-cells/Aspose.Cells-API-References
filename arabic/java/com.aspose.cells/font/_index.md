---
title: "Font"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف كائن الخط المستخدم في جدول بيانات."
type: docs
url: /ar/java/com.aspose.cells/font/
---

**Inheritance:**
java.lang.Object
```
public class Font
```

يغلف كائن الخط المستخدم في جدول بيانات.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Hello Aspose!");
 
         Font font = cell.getStyle().getFont();
 
         //Setting the font name to "Times New Roman"
         font.setName("Times New Roman");
 
         //Setting font size to 14
         font.setSize(14);
 
         //setting font color as Red
         font.setColor(com.aspose.cells.Color.getRed());           
 
         //Saving the Excel file
         workbook.save("dest.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | يتحقق مما إذا كان الخطان متساويين. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | يحصل على اللون بقيمة ARGB 32-بت. |
| [getCapsType()](#getCapsType--) | يحصل على نوع الحروف الكبيرة للنص. |
| [getCharset()](#getCharset--) | يمثل مجموعة الأحرف. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | يحصل على [Color](../../com.aspose.cells/color) للخط. |
| [getDoubleSize()](#getDoubleSize--) | يحصل على الحجم المزدوج للخط. |
| [getName()](#getName--) | يحصل على اسم الـ [Font](../../com.aspose.cells/font). |
| [getSchemeType()](#getSchemeType--) | يحصل على نوع المخطط للخط. |
| [getScriptOffset()](#getScriptOffset--) | يحصل على إزاحة النص، بوحدة النسبة المئوية |
| [getSize()](#getSize--) | يحصل على حجم الخط. |
| [getStrikeType()](#getStrikeType--) | يحصل على نوع الضربة للنص. |
| [getThemeColor()](#getThemeColor--) | يحصل على لون السمة. |
| [getUnderline()](#getUnderline--) | يحصل على نوع تسطير الخط. |
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
| [setCapsType(int value)](#setCapsType-int-) | يضبط نوع الحروف الكبيرة للنص. |
| [setCharset(int value)](#setCharset-int-) | يمثل مجموعة الأحرف. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | يضبط الـ[Color](../../com.aspose.cells/color) للخط. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | يضبط الحجم المزدوج للخط. |
| [setItalic(boolean value)](#setItalic-boolean-) | يضبط قيمة تشير إلى ما إذا كان الخط مائلًا. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم الـ [Font](../../com.aspose.cells/font). |
| [setName(String name, int type)](#setName-java.lang.String-int-) | يضبط الاسم والمخطط للخط. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | يشير إلى ما إذا كان تطبيع الارتفاع سيُطبق على مقطع النص. |
| [setSchemeType(int value)](#setSchemeType-int-) | يضبط نوع المخطط للخط. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | يضبط إزاحة النص، بوحدة النسبة المئوية |
| [setSize(int value)](#setSize-int-) | يضبط حجم الخط. |
| [setStrikeType(int value)](#setStrikeType-int-) | يحصل على نوع الضربة للنص. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | يضبط قيمة تشير إلى ما إذا كان الخط يحتوي على خط مشطوب واحد. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | يضبط قيمة تشير إلى ما إذا كان الخط مكتوبًا كمنخفض. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | يضبط قيمة تشير إلى ما إذا كان الخط مكتوبًا كمرتفع. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | يضبط لون السمة. |
| [setUnderline(int value)](#setUnderline-int-) | يضبط نوع تسطير الخط. |
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


يحصل على نوع الحروف الكبيرة للنص.

انظر [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

خاص فقط بخطوط الأشكال أو المخططات. ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--) . ستتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم الـ [Font](../../com.aspose.cells/font).

**Remarks**

إذا تم استخدام هذه الخاصية لتعيين اسم الخط، فسيتم تحديث [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) إلى [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE).

**Returns:**
java.lang.String
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
### getSize() {#getSize--}
```
public int getSize()
```


يحصل على حجم الخط.

**Returns:**
int
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

خاص فقط بخطوط الأشكال أو المخططات. ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--) . ستتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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


يضبط نوع الحروف الكبيرة للنص.

انظر [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

خاص فقط بخطوط الأشكال أو المخططات. ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--) . ستتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان الخط مائلًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم الـ [Font](../../com.aspose.cells/font).

**Remarks**

إذا تم استخدام هذه الخاصية لتعيين اسم الخط، فسيتم تحديث [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) إلى [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE).

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

خاص فقط بخطوط الأشكال أو المخططات. ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--) . ستتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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

