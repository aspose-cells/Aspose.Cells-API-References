---
title: "IndividualFontConfigs"
second_title: "Aspose.Cells for Java API 参考"
description: "每个对象的字体配置。"
type: docs
url: /zh/java/com.aspose.cells/individualfontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class IndividualFontConfigs
```

每个 [Workbook](../../com.aspose.cells/workbook) 对象的字体配置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [IndividualFontConfigs()](#IndividualFontConfigs--) | 构造函数。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontSources()](#getFontSources--) | 获取包含来源列表的数组的副本 |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | 返回一个数组，包含在原始字体不存在时使用的字体替代名称。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | 设置字体的专属来源。 |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | 设置字体文件夹 |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | 设置字体文件夹 |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | 设置字体来源。 |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | 为给定的原始字体名称设置字体替代名称。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### IndividualFontConfigs() {#IndividualFontConfigs--}
```
public IndividualFontConfigs()
```


构造函数。

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
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


获取包含来源列表的数组的副本

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public String[] getFontSubstitutes(String originalFontName)
```


返回一个数组，包含在原始字体不存在时使用的字体替代名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - 如果原始字体不存在，则使用的字体替代名称数组。
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


设置字体的专属来源。仅使用来源中的字体。

**Remarks**

System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") 如果已设置，将被忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | 包含 TrueType 字体的来源数组。 |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public void setFontFolder(String fontFolder, boolean recursive)
```


设置字体文件夹

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFolder | java.lang.String | 包含 TrueType 字体的文件夹。 |
| recursive | boolean | 确定是否扫描子文件夹。 |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public void setFontFolders(String[] fontFolders, boolean recursive)
```


设置字体文件夹

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFolders | java.lang.String[] | 包含 TrueType 字体的文件夹集合。 |
| recursive | boolean | 确定是否扫描子文件夹。 |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public void setFontSources(FontSourceBase[] sources)
```


设置字体来源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | 包含 TrueType 字体的来源数组。 |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


为给定的原始字体名称设置字体替代名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| originalFontName | java.lang.String | 原始字体名称。 |
| substituteFontNames | java.lang.String[] | 在原始字体不存在时使用的字体替代名称列表。 |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

