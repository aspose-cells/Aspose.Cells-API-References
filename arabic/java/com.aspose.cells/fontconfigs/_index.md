---
title: "FontConfigs"
second_title: "Aspose.Cells for Java API Reference"
description: "يحدد إعدادات الخط"
type: docs
url: /ar/java/com.aspose.cells/fontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class FontConfigs
```

يحدد إعدادات الخط
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FontConfigs()](#FontConfigs--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefaultFontName()](#getDefaultFontName--) | يحصل على اسم الخط الافتراضي. |
| [getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)](#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-) | احصل على معلومات بيانات ملف الخط. |
| [getFontSources()](#getFontSources--) | يحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | يرجع مصفوفة تحتوي على أسماء الخطوط البديلة التي تُستخدم إذا لم يكن الخط الأصلي موجودًا. |
| [hashCode()](#hashCode--) |  |
| [isFontAvailable(String fontName)](#isFontAvailable-java.lang.String-) | يشير إلى ما إذا كان الخط متاحًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | يضبط اسم الخط الافتراضي. |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | يضبط مصادر الخط الحصرية. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | يضبط مجلد الخطوط |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | يضبط مجلد الخطوط |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | يضبط مصادر الخط. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | أسماء بدائل الخط للاسم الأصلي للخط المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontConfigs() {#FontConfigs--}
```
public FontConfigs()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultFontName() {#getDefaultFontName--}
```
public static String getDefaultFontName()
```


يحصل على اسم الخط الافتراضي.

**Returns:**
java.lang.String
### getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle) {#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-}
```
public static FontFileDataInfo getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)
```


احصل على معلومات بيانات ملف الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontName | java.lang.String | اسم الخط |
| isBold | boolean | ما إذا كان نمط الخط غامقًا أم لا |
| isItalic | boolean | ما إذا كان نمط الخط مائلًا أم لا |
| isExactStyle | boolean | ما إذا كان يجب مطابقة نمط الغامق/المائل المحدد تمامًا |

**Returns:**
[FontFileDataInfo](../../com.aspose.cells/fontfiledatainfo) - Data infomation of font file data.
### getFontSources() {#getFontSources--}
```
public static FontSourceBase[] getFontSources()
```


يحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public static String[] getFontSubstitutes(String originalFontName)
```


يرجع مصفوفة تحتوي على أسماء الخطوط البديلة التي تُستخدم إذا لم يكن الخط الأصلي موجودًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - مصفوفة تحتوي على أسماء بدائل الخط لاستخدامها إذا لم يتم تقديم الخط الأصلي.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFontAvailable(String fontName) {#isFontAvailable-java.lang.String-}
```
public static boolean isFontAvailable(String fontName)
```


يشير إلى ما إذا كان الخط متاحًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontName | java.lang.String | اسم الخط |

**Returns:**
boolean - true إذا كان الخط متاحًا، وإلا false.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public static void setDefaultFontName(String value)
```


يضبط اسم الخط الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
```


يضبط مصادر الخط الحصرية. سيتم استخدام الخطوط الموجودة فقط في المصادر.

**Remarks**

System.setProperty(\"Aspose.Cells.FontDirExc\", \"fontExclusiveFolder\") سيتم تجاهله إذا تم ضبط هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | مصفوفة من المصادر التي تحتوي على خطوط TrueType. |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


يضبط مجلد الخطوط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontFolder | java.lang.String | المجلد الذي يحتوي على خطوط TrueType. |
| recursive | boolean | يحدد ما إذا كان يجب فحص المجلدات الفرعية أم لا. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


يضبط مجلد الخطوط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontFolders | java.lang.String[] | المجلدات التي تحتوي على خطوط TrueType. |
| recursive | boolean | يحدد ما إذا كان يجب فحص المجلدات الفرعية أم لا. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontSources(FontSourceBase[] sources)
```


يضبط مصادر الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | مصفوفة من المصادر التي تحتوي على خطوط TrueType. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public static void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


أسماء بدائل الخط للاسم الأصلي للخط المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| originalFontName | java.lang.String | اسم الخط الأصلي. |
| substituteFontNames | java.lang.String[] | قائمة بأسماء خطوط الاستبدال التي سيتم استخدامها إذا لم يتوفر الخط الأصلي. |

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

