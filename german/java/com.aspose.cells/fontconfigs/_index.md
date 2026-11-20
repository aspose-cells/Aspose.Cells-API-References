---
title: "FontConfigs"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Gibt Schriftarteinstellungen an"
type: docs
url: /de/java/com.aspose.cells/fontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class FontConfigs
```

Gibt Schriftarteinstellungen an
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FontConfigs()](#FontConfigs--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefaultFontName()](#getDefaultFontName--) | Liefert den Standard‑Schriftartnamen. |
| [getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)](#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-) | Ruft Dateninformationen der Schriftdatei ab. |
| [getFontSources()](#getFontSources--) | Liefert eine Kopie des Arrays, das die Liste der Quellen enthält. |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Gibt ein Array zurück, das Schriftart-Ersatznamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist. |
| [hashCode()](#hashCode--) |  |
| [isFontAvailable(String fontName)](#isFontAvailable-java.lang.String-) | Gibt an, ob die Schriftart verfügbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Legt den Standard-Schriftartnamen fest. |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Legt die exklusiven Quellen der Schriftarten fest. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Legt den Schriftarten-Ordner fest |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Legt den Schriftarten-Ordner fest |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Legt die Schriftart-Quellen fest. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Schriftart-Ersatznamen für den angegebenen Originalschriftartnamen. |
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
| Parameter | Typ | Beschreibung |
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


Liefert den Standard‑Schriftartnamen.

**Returns:**
java.lang.String
### getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle) {#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-}
```
public static FontFileDataInfo getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)
```


Ruft Dateninformationen der Schriftdatei ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontName | java.lang.String | Schriftartname |
| isBold | boolean | Der Schriftstil ist fett oder nicht |
| isItalic | boolean | Der Schriftstil ist kursiv oder nicht |
| isExactStyle | boolean | Ob der angegebene fett/kursiv-Stil exakt übereinstimmen soll |

**Returns:**
[FontFileDataInfo](../../com.aspose.cells/fontfiledatainfo) - Data infomation of font file data.
### getFontSources() {#getFontSources--}
```
public static FontSourceBase[] getFontSources()
```


Liefert eine Kopie des Arrays, das die Liste der Quellen enthält.

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public static String[] getFontSubstitutes(String originalFontName)
```


Gibt ein Array zurück, das Schriftart-Ersatznamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - Ein Array, das Schriftart-Ersatznamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist.
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


Gibt an, ob die Schriftart verfügbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontName | java.lang.String | Schriftartname |

**Returns:**
boolean - true, wenn die Schriftart verfügbar ist, sonst false.
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


Legt den Standard-Schriftartnamen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
```


Legt die exklusiven Quellen der Schriftarten fest. Nur Schriftarten in den Quellen werden verwendet.

**Remarks**

System.setProperty(\"Aspose.Cells.FontDirExc\", \"fontExclusiveFolder\") wird ignoriert, wenn dies gesetzt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Ein Array von Quellen, die TrueType-Schriftarten enthalten. |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Legt den Schriftarten-Ordner fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolder | java.lang.String | Der Ordner, der TrueType-Schriftarten enthält. |
| rekursiv | boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Legt den Schriftarten-Ordner fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Die Ordner, die TrueType-Schriften enthalten. |
| rekursiv | boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontSources(FontSourceBase[] sources)
```


Legt die Schriftart-Quellen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Ein Array von Quellen, die TrueType-Schriftarten enthalten. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public static void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Schriftart-Ersatznamen für den angegebenen Originalschriftartnamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| originalFontName | java.lang.String | Ursprünglicher Schriftname. |
| substituteFontNames | java.lang.String[] | Liste von Ersatzschriftartnamen, die verwendet werden, wenn die ursprüngliche Schrift nicht vorhanden ist. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

