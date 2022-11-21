---
title: FontConfigs
second_title: Aspose.Cells for Java API Reference
description: Specifies font settings
type: docs
weight: 223
url: /java/com.aspose.cells/fontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class FontConfigs
```

Specifies font settings
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefaultFontName()](#getDefaultFontName--) | Gets or sets the default font name. |
| [getFontSources()](#getFontSources--) | Gets a copy of the array that contains the list of sources |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Returns array containing font substitute names to be used if original font is not presented. |
| [getPreferSystemFontSubstitutes()](#getPreferSystemFontSubstitutes--) | Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | For the description of this property, please see [getDefaultFontName()](../../com.aspose.cells/fontconfigs\#getDefaultFontName--) |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Sets the fonts folder |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Sets the fonts folders |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Sets the fonts sources. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Font substitute names for given original font name. |
| [setPreferSystemFontSubstitutes(boolean value)](#setPreferSystemFontSubstitutes-boolean-) | For the description of this property, please see [getPreferSystemFontSubstitutes()](../../com.aspose.cells/fontconfigs\#getPreferSystemFontSubstitutes--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
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


Gets or sets the default font name.

**Returns:**
java.lang.String
### getFontSources() {#getFontSources--}
```
public static FontSourceBase[] getFontSources()
```


Gets a copy of the array that contains the list of sources

**Returns:**
com.aspose.cells.FontSourceBase[] - 
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public static String[] getFontSubstitutes(String originalFontName)
```


Returns array containing font substitute names to be used if original font is not presented.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - An array containing font substitute names to be used if original font is not presented.
### getPreferSystemFontSubstitutes() {#getPreferSystemFontSubstitutes--}
```
public static boolean getPreferSystemFontSubstitutes()
```


Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false.

**Returns:**
boolean
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




### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public static void setDefaultFontName(String value)
```


For the description of this property, please see [getDefaultFontName()](../../com.aspose.cells/fontconfigs\#getDefaultFontName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Sets the fonts folder

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolder | java.lang.String | The folder that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Sets the fonts folders

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | java.lang.String[] | The folders that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontSources(FontSourceBase[] sources)
```


Sets the fonts sources.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | An array of sources that contain TrueType fonts. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public static void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Font substitute names for given original font name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | java.lang.String | Original font name. |
| substituteFontNames | java.lang.String[] | List of font substitute names to be used if original font is not presented. |

### setPreferSystemFontSubstitutes(boolean value) {#setPreferSystemFontSubstitutes-boolean-}
```
public static void setPreferSystemFontSubstitutes(boolean value)
```


For the description of this property, please see [getPreferSystemFontSubstitutes()](../../com.aspose.cells/fontconfigs\#getPreferSystemFontSubstitutes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

