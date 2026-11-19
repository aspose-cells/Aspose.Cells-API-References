---
title: "IndividualFontConfigs"
second_title: "Aspose.Cells for Java API Reference"
description: "إعدادات الخط لكل كائن."
type: docs
url: /ar/java/com.aspose.cells/individualfontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class IndividualFontConfigs
```

إعدادات الخط لكل كائن [Workbook](../../com.aspose.cells/workbook).
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [IndividualFontConfigs()](#IndividualFontConfigs--) | منشئ. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontSources()](#getFontSources--) | يحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | يعيد مصفوفة تحتوي على أسماء خطوط بديلة لاستخدامها إذا لم يتوفر الخط الأصلي. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | يضبط مصادر الخط الحصرية. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | يضبط مجلد الخطوط |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | يضبط مجلدات الخطوط |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | يضبط مصادر الخط. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | يضبط أسماء الخطوط البديلة لاسم خط أصلي معين. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### IndividualFontConfigs() {#IndividualFontConfigs--}
```
public IndividualFontConfigs()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontSources() {#getFontSources--}
```
public FontSourceBase[] getFontSources()
```


يحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public String[] getFontSubstitutes(String originalFontName)
```


يعيد مصفوفة تحتوي على أسماء خطوط بديلة لاستخدامها إذا لم يتوفر الخط الأصلي.

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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
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
public void setFontFolder(String fontFolder, boolean recursive)
```


يضبط مجلد الخطوط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontFolder | java.lang.String | المجلد الذي يحتوي على خطوط TrueType. |
| recursive | boolean | يحدد ما إذا كان يجب فحص المجلدات الفرعية أم لا. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public void setFontFolders(String[] fontFolders, boolean recursive)
```


يضبط مجلدات الخطوط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontFolders | java.lang.String[] | المجلدات التي تحتوي على خطوط TrueType. |
| recursive | boolean | يحدد ما إذا كان يجب فحص المجلدات الفرعية أم لا. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public void setFontSources(FontSourceBase[] sources)
```


يضبط مصادر الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | مصفوفة من المصادر التي تحتوي على خطوط TrueType. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


يضبط أسماء الخطوط البديلة لاسم خط أصلي معين.

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

